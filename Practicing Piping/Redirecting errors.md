# Redirecting errors
The aim of the challenge is to redirect the output of the command `/challenge/run` to `myflag` and the errors to `instructions`

## My solve
**Flag:** ` pwn.college{sbISkjxuJR8peDoHF5HRG9jPOBK.QX3YTN0wiN3AzNzEzW}`

```
hacker@piping~redirecting-errors:~$ /challenge/run 1> myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat instructions
.
.
.
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-errors:~$ cat myflag
[FLAG] Here is your flag:
[FLAG] pwn.college{sbISkjxuJR8peDoHF5HRG9jPOBK.QX3YTN0wiN3AzNzEzW}
```


## What I learned
Difference between redirecting output and errors to different files. For redirecting output, we make use of `>` and `2>` in case of outputs.
Using this helps us to not display error on the terminal when invoking a command.

## References 
reference material from pwn.college
