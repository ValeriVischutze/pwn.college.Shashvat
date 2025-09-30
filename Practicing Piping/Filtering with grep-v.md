# Filtering with grep-v
The aim of the challenge is to grep out the actual flag from a bunch of 1000 decoy flags.

## My solve
**Flag:** `pwn.college{Adqv1TdwBGzDo0KHXsJX2UtnRPC.0FOxEzNxwiN3AzNzEzW} 

```
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{Adqv1TdwBGzDo0KHXsJX2UtnRPC.0FOxEzNxwiN3AzNzEzW}
```
The `grep -v` command helps us to grep out terms that DO NOT follow the given pattern that is mentioned in argument. This helped us to highlight the flag by marking out all flags containing the DECOY. 

## What I learned
The application of the `grep -v` command.

## References 
Reference material from pwn.college
