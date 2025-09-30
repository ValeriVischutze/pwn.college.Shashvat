# Matching paths with []
Starting from your home directory, run /challenge/run with a single argument that bracket-globs into the absolute paths to the file_b, file_a, file_s, and file_h files!

## My solve
**Flag:** `pwn.college{kTd42wbf1ZBYi-8R1PFq_4frK6J.QX0IDO0wiN3AzNzEzW} `

```
/challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{kTd42wbf1ZBYi-8R1PFq_4frK6J.QX0IDO0wiN3AzNzEzW} 
```
In this challenge we run the /challenge/run with absolute path of files as /challenge/files/file[bash].

## What I learned
using [] glob with absolute path of the files.

## References 
Reference material from pwn.college
