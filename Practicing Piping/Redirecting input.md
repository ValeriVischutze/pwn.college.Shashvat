# Redirecting input
The aim of the challenge is to store `COLLEGE` into the `PWN` file before redirecting it to our command `/challenge/run` or making the `/challenge/run` take the `PWN` file as its input.

## My solve
**Flag:** `pwn.college{E99doeIVIqVEaqZryWnXPnIY26h.QXwcTN0wiN3AzNzEzW} `

```
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{E99doeIVIqVEaqZryWnXPnIY26h.QXwcTN0wiN3AzNzEzW}
```
firstly, we redirected the value of COLLEGE to the PWN file before redirecting it as an input for our command.

## What I learned
Simultaneous application of redirecting values and input

## References 
Reference material from pwn.college
