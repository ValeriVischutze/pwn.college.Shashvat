# Exclusionary globbing
cd to /challenge/files and run /challenge/run with all files that don't start with p, w, or n!

## My solve
**Flag:** `pwn.college{8IRCGblqJQ9Ev4aY3ydCHJsrVp8.QX2IDO0wiN3AzNzEzW}`

```
cd /challenge/files
/challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{8IRCGblqJQ9Ev4aY3ydCHJsrVp8.QX2IDO0wiN3AzNzEzW}
```
In this challenge we cd to /challenge/files the use ! to run /challenge/run with all the files not starting from p,w,n as /challenge/run [pwn]* .

## What I learned
! or ^ inverts the funtion of the glob used with.

## References 
Reference material from pwn.college
