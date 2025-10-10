# Hijacking commands
Armed with your knowledge, you can now carry out some shenanigans. This challenge is almost the same as the first challenge in this module. Again, this challenge will delete the flag using the rm command. But unlike before, it will not print anything out for you.
How can you solve this? You know that rm is searched for in the directories listed in the PATH variable. You have experience creating the win command when the previous challenge needed it.

## My solve
**Flag:** `pwn.college{Yzh_Sd1MWSJnaSk4v0de7FdRLKf.QX3cjM1wiN3AzNzEzW} `


```
mkdir -p /tmp/mybin
cat > /tmp/mybin/rm <<'SH'
/bin/cat /flag
exit 0
SH
chmod +x /tmp/mybin/rm
export PATH=/tmp/mybin:$PATH
/challenge/run
Trying to remove /flag...
Found 'rm' command at /tmp/mybin/rm. Executing!
pwn.college{Yzh_Sd1MWSJnaSk4v0de7FdRLKf.QX3cjM1wiN3AzNzEzW} 
```

## What I learned
I created the `rm` command such that it reads out the flag itself, then set PATH environment to where that rm command is

## References 
Reference material from pwn.college
