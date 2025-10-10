# The SUID bit
in this challenge, we will execute programs with SUID permission. The "Set User ID" (SUID) permissions bit allows the user to run a program as the owner of that program's file.

## My solve
**Flag:** `pwn.college{wczU_TBGJx02usSszbZuYV3ua19.QXzEjN0wiM5AzNzEzW}`

```
chmod a+s /challenge/getroot
/challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
cat /flag
pwn.college{wczU_TBGJx02usSszbZuYV3ua19.QXzEjN0wiM5AzNzEzW}
```

## What I learned
I can now add `+s` permissions to files such that the program becomes executable with SUID.

## References 
Reference material from pwn.college
