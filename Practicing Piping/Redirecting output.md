# Redirecting output
The challenge expects us to redirect the output of the given command to a given target file.

## My solve
**Flag:** `pwn.college{ov5Odptsy12z6or4qsH23YnveCH.QX0YTN0wiN3AzNzEzW} `
```
hacker@piping~redirecting-output:~$ echo PWN > COLLEGE
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your flag:
pwn.college{ov5Odptsy12z6or4qsH23YnveCH.QX0YTN0wiN3AzNzEzW}
```
by using the addition '>' in the echo command, we redirected the output "PWN" to the COLLEGE file.


## What I learned
basic redirection of text output to a given target file.

## References 
Reference material from pwn.college
