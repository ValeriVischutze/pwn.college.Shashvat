# Other users with su
With no arguments, su will start a root shell (after authenticating with root's password). However, you can also give a username as an argument to switch to that user instead of root.

## My solve
**Flag:** `pwn.college{INaUmb2Syijhw6B9SFr75vtaLTl.QX2UDN1wiN3AzNzEzW}`


```
hacker@users~other-users-with-su:~$ su zardus
Password: dont-hack-me
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{INaUmb2Syijhw6B9SFr75vtaLTl.QX2UDN1wiN3AzNzEzW}
```

## What I learned
giving username argument with `su` to switch to that user. 

## References 
Reference material from pwn.college
