# Making directories
create a /tmp/pwn directory and make a college file in it! Then run /challenge/run.

## My solve
**Flag:** `pwn.college{8EtFln4jifOs2YsuIWTVRo_6wBr.QXxMDO0wiN3AzNzEzW}`

Here, we first create the pwn directory in the /tmp directory before creating a file college in the pwn directory. Upon invoking the target command, we obtain the flag.
```
cd /tmp
/tmp$ mkdir pwn
/tmp$ cd /tmp/pwn
/tmp/pwn$ touch college
/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{8EtFln4jifOs2YsuIWTVRo_6wBr.QXxMDO0wiN3AzNzEzW}
```

## What I learned
The use of `mkdir` to create new directories

## References 
Reference material from pwn.college
