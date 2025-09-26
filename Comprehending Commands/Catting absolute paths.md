# Catting absolute paths
The aim of the challenge is the invoke a cat command through an absolute pathway.

## My solve:
**Flag:** `pwn.college{w7UNqsl1XcE5D-6Fw4yUywN0I1L.QX5ETO0wiN3AzNzEzW}`

`cat` just like any other command can be invoked through an absolute pathway. To invoke the flag variable, we use the `cat /flag` which is an absolute path (starting from the directory). 
Issuing this command invokes the flag.

## What I learned:
The application of `cat` command through an absolute path.

## References 
Reference video from pwn.college
