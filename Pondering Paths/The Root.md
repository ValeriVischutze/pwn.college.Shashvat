# The Root
The aim of this challenge is to familiarize with the basics of directories and invoke the basic directory command.

## My solve:
**Flag:** `pwn.college{c_8ID7fClMCF_YZ4zQZCeFY5j22.QX4cTO0wiN3AzNzEzW} `

A directory is essentially a file which holds or catalogues other files. A directory can essentially host many other sub directories, the root directory being 'ultimate' directory.
In the given challenge we already start with the root directory (which can also be invoked by issuing a ` cd /` command) and finally invoke the pwn command in the root directory, `/pwn` to obtain the flag.

## What I learned:
The basic idea surrounding the division of the system into directories of which the 'ultimate' directory is the root directory,a single directory to which all other directories can be traced back.

## References:
Reference video from pwn.college
