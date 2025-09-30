# Redirecting more output
The aim of the challenge is to learn how to extend the principle of redirecting output of a given command to a more generalized

## My solve
**Flag:** `pwn.college{AK3M9GQ3iTP0BTe5T29Aody_-je.QX1YTN0wiN3AzNzEzW}`

Just like in the previous challenge, using the '>' after our command enables us to redirect the ouput of this program to the given target file.
```
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
.
.
.
[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag
[FLAG] Here is your flag:
[FLAG] pwn.college{AK3M9GQ3iTP0BTe5T29Aody_-je.QX1YTN0wiN3AzNzEzW}
```


## What I learned
Further application of redirecting, past the basic redirecting.

## References 
Reference material from pwn.college
