# Becoming root with su
In this challenge, we will cover the older one, su (the substitute user command). 
This is not typically used to elevate to root access anymore, but it is an elegant utility from a more civilized time, and we'll cover it first.

## My solve
**Flag:** `pwn.college{EB0AefqNsWdmaLMTmC1Ve2-bhuf.QX1UDN1wiN3AzNzEzW}`


```
hacker@users~becoming-root-with-su:~$ su
password: hack-the-planet
root@users~becoming-root-with-su:/home/hacker# ls
root@users~becoming-root-with-su:/home/hacker# cat not-the-flag
pwn.college{EB0AefqNsWdmaLMTmC1Ve2-bhuf.QX1UDN1wiN3AzNzEzW}
```

## What I learned
`su` command to get root (administrative) access of your system

## References 
Reference material from pwn.college
