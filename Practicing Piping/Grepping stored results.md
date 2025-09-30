# Grepping stored results
The aim of the challenge is to first redirect the output of the `/challenge/run` command to the `/tmp/data.txt` before catching the flag from amidst a houndred thousand lines of output using the `grep` command.

## My solve
**Flag:** `pwn.college{Qzkkn1PZCoAx_L3SiVE7bSyEr2V.QX4EDO0wiN3AzNzEzW}`

```
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
.
.
.
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep 'pwn' /tmp/data.txt
pwns
pwn.college{Qzkkn1PZCoAx_L3SiVE7bSyEr2V.QX4EDO0wiN3AzNzEzW}
.
.
```
First we redirect the output of the command `/challenge/run` to the `/tmp/data.txt` file before grepping the flag by using the keyword `pwn` as every flag contains the `pwn.college` prefix.

## What I learned
Simultaneous redirection and application of the `grep` command to capture the flag.

## References 
Reference material from pwn.college
