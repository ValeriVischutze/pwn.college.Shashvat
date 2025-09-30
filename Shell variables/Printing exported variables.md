# Printing exported variables
The aim of the challenge is to familiarize with the `env` command.

## My solve
**Flag:** `pwn.college{cPrBSNNW2ZzT2WnsWj2R7LbldpE.QX4UTN0wiN3AzNzEzW}`

```
hacker@variables~printing-exported-variables:~$ env
SHELL=/run/dojo/bin/bash
.
.
.
FLAG=pwn.college{cPrBSNNW2ZzT2WnsWj2R7LbldpE.QX4UTN0wiN3AzNzEzW}
.
.
.
```

## What I learned
env command prints all the exported variables set in the shell.

## References 
Reference material from pwn.college
