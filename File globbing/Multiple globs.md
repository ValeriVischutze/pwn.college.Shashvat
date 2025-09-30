# Multiple globs
cd to /challenge/files and run /challenge/run, providing a single argument: a short (3 characters or less) globbed word with two * globs in it that covers every word that contains the letter p.

## My solve
**Flag:** `pwn.college{Uf2JxoiyUxjQAfmvQus4RRpGdgO.0lM3kjNxwiN3AzNzEzW}`

```
cd /challenge/files
/challenge/run *p*
You got it! Here is your flag!
pwn.college{Uf2JxoiyUxjQAfmvQus4RRpGdgO.0lM3kjNxwiN3AzNzEzW}
```
In this challenge we changed directory to /challenge/files then run the /challenge/run with two * globs and single argument p as /challenge/run p

## What I learned
multiple globs for a single argument.

## References 
Reference material from pwn.college
