# Searching manuals
The aim of the challenge is browse through the challenge manual and find the correct argument to use with the target command and invoke the flag.

## My solve:
**Flag:** `pwn.college{khG1t73dxwiDs-NHLI-y4ubwCFC.QX1EDO0wiN3AzNzEzW} `

We invoke the `man challenge` command to go through the manual of the `challenge` directory. Here, we come across a list of several arguments of which one when used ewith the target command enables us to obtain the flag.
For this, we make use of the `?` or the `/` commands in the `challenge` manual.
In my case I used `/flag`, essentially to highlight the only argument that lead to the flag.

```
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --wkvth
Initializing...
Correct usage! Your flag: pwn.college{khG1t73dxwiDs-NHLI-y4ubwCFC.QX1EDO0wiN3AzNzEzW}
```
After using `/flag` in the challenge manual:
```
--wkvth 
This argument will give you the flag!
```



## What I learned:
How to browse through a given challenge manual to find the target argument by searching with keywords.

## References 
Reference material from pwn.college
