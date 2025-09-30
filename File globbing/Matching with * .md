# Matching with *
Starting from your home directory, change your directory to /challenge, but use globbing to keep the argument you pass to cd to at most four characters! Once you're there, run /challenge/run for the flag!

## My solve
**Flag:** `pwn.college{wIFiTYV1Bvnk1RNAE-C8VmCRiI8.QXxIDO0wiN3AzNzEzW}`

```
cd /*ge
/challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{wIFiTYV1Bvnk1RNAE-C8VmCRiI8.QXxIDO0wiN3AzNzEzW} 
```


In this challenge we changed directory to /challenge using * Glob as cd /*ge.


## What I learned
Glob * it replaces the argument that matches any pattern.

## References 
Reference material from pwn.college
