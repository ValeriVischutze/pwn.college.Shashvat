## The PATH variable
In this level, we will disrupt the operation of the /challenge/run program. This program will DELETE the flag file using the rm command.
However, if it can't find the rm command, the flag will not be deleted, and the challenge will give it to you! Thus, you must make it so that /challenge/run also can't find the rm command.

### My Solve:
**Flag:** `pwn.college{EVLAA-JcJu4NvJHVUUFzvvVzs5l.QX2cDM1wiN3AzNzEzW}`

```
mkdir -p /tmp/empty
export PATH=/tmp/empty
/challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: command not found
The flag is still there! I might as well give it to you!
pwn.college{EVLAA-JcJu4NvJHVUUFzvvVzs5l.QX2cDM1wiN3AzNzEzW}
```

### What I learnt:
PATH command to redirect shell command directories

### References:
Reference material from pwn.college
