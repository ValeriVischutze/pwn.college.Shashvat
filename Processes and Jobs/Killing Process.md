# Killing Process
The aim of the challenge is to first halt the `/challenge/dont_run` command before running the `/challenge/run` command to obtain the flag.

## My solve
**Flag:** `pwn.college{YPcAy05R52crVzE_3TAWEUigFg9.QXyQDO0wiN3AzNzEzW}`

We use ps command with argument aux to see the PID of `/challenge/dont_run` then used kill command to terminate the process as `kill PID_/challenge/dont_run`.
```
hacker@processes~killing-processes:~$ ps aux
.
.
hacker       136  0.0  0.0 231576  3520 ?        Ss   12:46   0:00 /challenge/dont_run
.
.
hacker       155  0.0  0.0   5656  2880 pts/0    S+   12:47   0:00 /bin/bash /challenge/dont_run
.
.
kill 136
kill 155
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{YPcAy05R52crVzE_3TAWEUigFg9.QXyQDO0wiN3AzNzEzW}
```

## What I learned
We cannot directly use the `/challenge/run` command whilst the `/challenge/dont_run` runs in the background. To terminate it first, we use the `kill` command.

## References 
Reference material from pwn.college.
