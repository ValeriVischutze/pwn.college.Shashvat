# Interrupting Processes
The aim of this challenge is to first override the interruption stopping us from invoking the flag

## My solve
**Flag:** `pwn.college{IlL1PYqJymj0S-RcifY9F3-dYa_.QXzQDO0wiN3AzNzEzW}`

We invoke the `/challenge/run` command, but it'll be interrupted by a warning message. To override it, we use ctrl+c.
```
hacker@processes~interrupting-processes:~$ /challenge/run
I could give you the flag... but I won't, until this process exits. Remember,
you can force me to exit with Ctrl-C. Try it now!
^C
Good job! You have used Ctrl-C to interrupt this process! Here is your flag:
pwn.college{IlL1PYqJymj0S-RcifY9F3-dYa_.QXzQDO0wiN3AzNzEzW}
```

## What I learned
ctrl-C interrupts the process running. It causes the application to cleanly exit.

## References 
Reference material from pwn.college
