# Explicit relative paths
The aim of the challenge is to execute the target code by using an explicit relative pathway (from the root directory)

## My solve:
**Flag** `pwn.college{YrDPQ_zJ5czOilr3klsZH-_qau_.QXwUTN0wiN3AzNzEzW} `

We switch to the root directory using the `cd /` command before invoking the `./challenge/run` with '.' being an explicit entry which stands for "in this given directory".
Essentially this commands can be translated as:" in this (or root directory) directory, move to the challenge directory and execute the command run"
This challenge avoids the more 'descending' route to execute the command .i.e. by descending from a given directory (in our case here, the root directory) to the intended directory and executing the code.

## What I learned:
The difference between an explicit and implicit relative pathway. An explicit path would make use of '.', which means 'in the current directory', and '..' meaning 'to the parent directory.'

## References
Reference video from pwn.college
