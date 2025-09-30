# Finding files
The aim of the challenge is to find the flag hidden in an arbitrary filesystem. 

## My solve
**Flag:** `pwn.college{YwCwHdiSqlFp9Wzxr6IbPdx81rL.QXyMDO0wiN3AzNzEzW}`


```
find / -name flag
.
.
.
/usr/local/lib/python3.8/dist-packages/pwnlib/flag 
/usr/lib/debug/.build-id/6d/flag
cat /usr/lib/debug/.build-id/6d/flag
pwn.college{YwCwHdiSqlFp9Wzxr6IbPdx81rL.QXyMDO0wiN3AzNzEzW}
```
In this challenge we simply employed the searching method by using the find command

## What I learned
The application of the find command as an effective searching tool

## References 
Reference material from pwn.college
