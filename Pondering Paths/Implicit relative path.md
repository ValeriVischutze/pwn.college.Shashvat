# Implicit relative path
The aim of the challenge is to invoke the target command in the given directory by using an implicit pathway however by avoiding to execute other commands that happen to have the same name in the system.

## My solve:
**Flag** `pwn.college{EaxSoSR2PTV3uTBtx3GncNp4_3R.QXxUTN0wiN3AzNzEzW} `

This challenge is quite a classic which makes it so fascinating to solve...It explains why we use the `.` .We use the `cd /challenge` command to shift to the challenge directory. Now to invoke our target command we issue the `./run` command.
The logic behind this is that there can be other commands in the utilities of the system that'll share the same name as our target command. As such, to avoid executing those other commands should we proceed with `cd /challenge` and `run`, bash displays an error message about the command not being found.
Using `./run` would ensure that the command is belonging to the `/challenge` directory.

## What I learned:
The reasoning behind using `.` in an implicit pathway, and avoiding semantic errors.

## References:
Reference video from pwn.college
