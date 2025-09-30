# Grepping live outputs
The aim of the challenge is to redirect the output of the `/challenge/run` command, without storing it in a file, before capturing the flag using the `grep` command

## My solve
**Flag:** `pwn.college{kKPJ_3spvCAfUGKMUlqtzGCZaXY.QX5EDO0wiN3AzNzEzW}`

```
hacker@piping~grepping-live-output:~$ /challenge/run | grep 'pwn'
.
.
.
[PASS] Success! You have satisfied all execution requirements.
pwns
.
.
pwn.college{kKPJ_3spvCAfUGKMUlqtzGCZaXY.QX5EDO0wiN3AzNzEzW}
```
We use piping (`|`) to avoid first redirecting the output of the command to a given file and then seperately grepping the flag.

## What I learned
Simultaneous storing and grepping of the flag through the piping operator.

## References 
Reference material from pwn.college
