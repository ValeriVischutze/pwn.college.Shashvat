# Grepping errors
The aim of the challenge is to first 'pipe' the error before grepping the flag.

## My solve
**Flag:** `pwn.college{8ABFLI0gDeryBgujQ1fzJG2-RS4.QX1ATO0wiN3AzNzEzW}`

```
hacker@piping~grepping-errors:~$ /challenge/run 2>&1 | grep 'pwn'
.
.
.
[PASS] Success! You have satisfied all execution requirements.
pwn.college{8ABFLI0gDeryBgujQ1fzJG2-RS4.QX1ATO0wiN3AzNzEzW}
.
.
.
```
We cannot directly use the piping command for redirecting errors. So instead we first convert the `stderr` to `stout` using the `2>&1` before it can be piped out, before grepping the flag.

## What I learned
How to convert `stderr` to `stdout`.

## References 
Reference material from pwn.college
