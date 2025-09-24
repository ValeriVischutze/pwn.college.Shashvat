# Program and Absolute Paths
The challenge is about executing a given command in a directory called the Challenge Directory

## My solve:
**Flag:** pwn.college{Mq1eFNlQ7LtCEJccurNQaEXnS81.QX1QTN0wiN3AzNzEzW} 
For solving the challenge, we first had to move to the root directory, to which all other directories in the sytem can be traced. For that we use the `cd /` command.
Now after moving the root directory, we switch to the challenge directory by issuing the `cd /challenge` command. Once in this directory, we execute the task of invoking the `/challenge/run` command and hence obtain our flag.

## What I learned:
Through this challenge, One can primarily learn how to switch and run commands in a given target directory.

## References:
Reference video from pwn.college
