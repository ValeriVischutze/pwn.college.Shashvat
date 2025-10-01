# Tab completion
Aim: this challenge has copied the flag into /challenge/pwncollege, and you can freely cat that file. But you can't type the filename: we used some serious trickery to make sure that you must tab-complete it. 

## My solve
**Flag:** `pwn.college{87X7FpJTdIpMp9wTkmCNFjITYmI.0FN0EzNxwiN3AzNzEzW}`


```
cat /cha<TAB>/pwnco<TAB>
pwn.college{87X7FpJTdIpMp9wTkmCNFjITYmI.0FN0EzNxwiN3AzNzEzW} 
```
Clicking on tab as we're writing the commands, sort of auto expands them to fit the nearest word, just like how google search works.

## What I learned
Tab key can expand the name which we are writting.

## References 
Reference material from pwn.college
