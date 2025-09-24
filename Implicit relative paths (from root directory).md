# Implicit relative paths (from the root directory)
The challenge is to invoke the command by taking a relative pathway.

## My solve:
**Flag** `pwn.college{8VP3o6IOqNDKnt7YW94WA229NJx.QX5QTN0wiN3AzNzEzW} `

Firstly we switch to the root directory using `cd /`. Once here, we invoke `challenge/run` which helps us obtain the flag. 
Using `/challenge/run` would've been an abolute path, which when dissecting the command can be read as,'in the root directory there is a challenge directory which further leads to the command run'.

# What I learned:
Absolute commands are issued w.r.t the root directory and need the reference of the complete path taken (from the root directory) to reach the intended command. 
A relative command as the term suggests, can be issued w.r.t to any given directory from which we intend take as a reference.

# References:
Reference video from pwn.college
