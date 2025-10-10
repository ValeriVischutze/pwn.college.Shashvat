# Cracking Passwords
The aim of the challenge is to learn how to decrupt passwords using the `john` command.

## My solve
**Flag:** `pwn.college{gbhvjW9pfNCjnrt5b81yZDyWSU2.QX3UDN1wiN3AzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible.. Use triple ticks for bash.
```bash
hacker@users~cracking-passwords:~$ cd /challenge
hacker@users~cracking-passwords:/challenge$ john shadow-leak
Created directory: /home/hacker/.john
.
.
.
hacker@users~cracking-passwords:/challenge$ john shadow-leak --show
hacker:NO PASSWORD:20357:0:99999:7:::
zardus:aardvark:20371:0:99999:7:::
2 password hashes cracked, 0 left
hacker@users~cracking-passwords:/challenge$ su zardus
Password: aardvark
zardus@users~cracking-passwords:/challenge$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{gbhvjW9pfNCjnrt5b81yZDyWSU2.QX3UDN1wiN3AzNzEzW}
```

## What I learned
I can now crack encrypted passwords (like a true goat ;) ).

## References 
Reference material from pwn.college
