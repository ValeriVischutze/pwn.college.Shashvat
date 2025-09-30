# Process substituion for input
The aim of the challenge is to differentiate between two given set of files and find out the actual flag. 

## My solve
**Flag:** `pwn.college{U4zRSqPXEm9nBDBXUnY4NaAsUEL.0lNwMDOxwiN3AzNzEzW}`

```
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
67a68
> pwn.college{U4zRSqPXEm9nBDBXUnY4NaAsUEL.0lNwMDOxwiN3AzNzEzW}
```
we use process substitution to save the output of a given file into a temporary file. The temporary file will read the data from the `stdout` of the file that has to be substituted for.

## What I learned
The basics of process substitution

## References 
Reference material from pwn.college
