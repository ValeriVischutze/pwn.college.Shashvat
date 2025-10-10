# Using sudo
In this challenge we will learn about `sudo` command to gain system-wide access to files and directories.

## My solve
**Flag:** `pwn.college{QgE6yXfeJ33uAnZWslsWv1yc6-p.QX4UDN1wiN3AzNzEzW}`

```
hacker@users~using-sudo:~$ ls
hacker@users~using-sudo:~$ cat not-the-flag
cat: not-the-flag: Permission denied
hacker@users~using-sudo:~$ sudo cat not-the-flag
pwn.college{QgE6yXfeJ33uAnZWslsWv1yc6-p.QX4UDN1wiN3AzNzEzW}
```

## What I learned
`sudo` used a prefix over other commands, can help us gain temporary access to the root.

## References 
reference material from pwn.college
