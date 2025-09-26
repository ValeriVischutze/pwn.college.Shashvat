# Hidden files
The aim of the challenge is to find the flag, which is stored in the root directory as a hidden file.

## My solve:
**Flag:** `pwn.college{gknk0uRdiMrNjIYyUqVRmGdkppV.QXwUDO0wiN3AzNzEzW} `

To solve this challenge, we switched to the root directory using `cd /`, before invoking the `ls -a`, which enables us to view the hidden files stored in the directory. Upon doing so, we uncover the hidden file leading 
to the flag, before invoking the `cat .flag-51981840112485` to obtain the flag variable.

## What I learned:
Not all files of a directory are visible to us. Hidden files are stored in the `.flag-51981840112485`type format and can be accessed in the same format. To access hidden files, we view these hidden files we use the `ls -a` command.

## References:
Reference material from pwn.college
