# Changing file ownership 
In this level, we will practice changing the owner of the /flag file to the hacker user, and then read the flag. For this challenge only, 
I made it so that you can use chown to your heart's content as the hacker user (again, typically, this requires you to be root).

## My solve
**Flag:** `pwn.college{UcpjqDVZX8Vo6_pyf0YPgygjw55.QXxEjN0wiN3AzNzEzW}`

```
cd /
chown hacker flag
cat flag
pwn.college{UcpjqDVZX8Vo6_pyf0YPgygjw55.QXxEjN0wiN3AzNzEzW} 
```

## What I learned
i can now change file ownership for various files.

## References 
Reference material from pwn.college
