# Group and Files
In this challenge we will how to change group ownership for a file

## My solve
**Flag:** `pwn.college{wVQb8SYTF6ZUoXx9pLBHHRd52zU.QXxcjM1wiN3AzNzEzW}`

```
id
uid=1000(hacker) gid=1000(hacker) groups=1000(hacker)
cd /
ls -l flag
-r--r----- 1 root root 60 Oct 10 18:07 flag
chgrp hacker flag
cat flag
pwn.college{wVQb8SYTF6ZUoXx9pLBHHRd52zU.QXxcjM1wiN3AzNzEzW} 
```

## What I learned
i can now change group ownership of files using `chgrp` command.

## References 
Reference material from pwn.college
