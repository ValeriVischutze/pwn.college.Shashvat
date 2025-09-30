# Matching with []
Change your working directory to /challenge/files and run /challenge/run with a single argument that bracket-globs into file_b, file_a, file_s, and file_h!

## My solve
**Flag:** `pwn.college{wjEvJ8rmAyuCuKdIlzbOfZVExe-.QXzIDO0wiN3AzNzEzW}`


```
cd /challenge/files
/challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{wjEvJ8rmAyuCuKdIlzbOfZVExe-.QXzIDO0wiN3AzNzEzW}
```
In this challenge we changed directory to /challenge/files run /challenge/run with [] glob as /challeng/run file_[bash].

## What I learned
Glob [] it is a limited form of ? glob it access the single characters of files specified inside [].

## References 
Reference material from pwn.college
