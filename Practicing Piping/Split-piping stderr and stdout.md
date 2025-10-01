# Split-piping stderr and stdout 
Aim:
• /challenge/hack: this produces data on stdout and stderr 
• /challenge/the: you must redirect hack's stderr to this program 
• /challenge/planet: you must redirect hack's stdout to this program

## My solve
**Flag:** `pwn.college{8ninkkhZyX_C0xAxIyoVUejvhEO.QXxQDM2wiN3AzNzEzW}`

Here we redirected the standard error of /challenge/hack to /challenge/the using 2< then redirected standard output of /challenge/hack to /challenge/planet
using >() and | pipe operator because when >() used on /challenge/the it did not redirect the standard error to /challenge/planet.
/challenge/hack 2> >(/challenge/the) | /challenge/planet
```
/challenge/hack 2> >(/challenge/the) | /challenge/planet
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{8ninkkhZyX_C0xAxIyoVUejvhEO.QXxQDM2wiN3AzNzEzW}
```

## What I learned
Learnt to redirect stderr to one program and stdout to another using combination of 2>,>() and | operators.

## References 
Reference material from pwn.college
