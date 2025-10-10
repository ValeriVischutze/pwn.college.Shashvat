# Listing processes
The aim of the challenge is to find the flag using the running list before running the command to obtain it.

## My solve
**Flag:** `pwn.college{gFVxCDKXUPLwA6n3IdcyIpiTzpU.QX4MDO0wiN3AzNzEzW}`

We obtain all the files running using ps command with argument `-ef` as `ps -ef` then read the running `/challenge/run` file which was renamed as `/challenge/6428-run-6916`.
```
hacker@processes~listing-processes:~$ ps -he
.
.
.
root         132       1  0 12:04 ?        00:00:00 /challenge/6428-run-6916
.
.
.
hacker@processes~listing-processes:~$ /challenge/6428-run-6916
Yahaha, you found me! Here is your flag:
pwn.college{gFVxCDKXUPLwA6n3IdcyIpiTzpU.QX4MDO0wiN3AzNzEzW}
Now I will sleep for a while (so that you could find me with 'ps')
```

## What I learned
ps command and arguments -ef and aux.

## References 
Reference material from pwn.college
