# Removing files
The aim of the challenge was to familiarize with how to delete files

## My solve:
**Flag:** `pwn.college{Qql1F1SZjom9cE_avPzRKWUjxUd.QX2kDM1wiN3AzNzEzW}`

To delete a file, we invoke the `rm` command. In this challenge, we invoke the remove command `rm delete_me` (a file which was already created in the home directory as the challenge was started), to delete the file.
We then invoke `/challenge/check` as a verification for the successful execution of the command and hence obtained the flag.

## What I learned:
How to delete files from a directory.

## References 
Reference material from pwn.college
