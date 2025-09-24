# Position thy self
The aim of the challenge is to execute a given command from a specific path set in the challenge directory.

## My solve:
**Flag:** `pwn.college{EJZ72llWGe1cXNShMx5KkYNXKYp.QX2QTN0wiN3AzNzEzW} `

Firstly we check out switch to the challenge directory by issuing the change directory command, `cd /challenge` .
Now we use the `ls` command to list out the contents of the challenge directory as a step to locate the challenge conditions. Upon using this command we come across a `DESCRIPTION.md run` file, which means that to access its contents we will issue the `cat` command.
Upon using the `cat run` command, we come across a list of certain 'Candidate directories', one of which will invoke the flag if we execute the intended target `/challenge/run` command.
By accessing the one of these directories , for eg. the `/var` directories, the shell issues a message `Incorrect...You're not currently in the / directory`, which implies that the target command has to be executed in the root directory itself.
Upon doing so we obtain out flag.

### What I learned:
To obtain the given challenge condition and position myself in the given target directory from where we've to issue the command.

# References:
Reference video from pwn.college
