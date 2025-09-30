# Appending output
The aim of the challenge is to append the output of the command `/challenge/run` to `the-flag` file in the home directory.

## My solve
**Flag:** `pwn.college{4PaTtyUK-DiFvDHSfBIJN7JGPdg.QX3ATO0wiN3AzNzEzW}`

Using '>>' enables us to append output to a file. According to our problem, the first half of the flag is already in `the-flag` file.
Now, using it over '>' here is because the '>' would overwrite `the-flag` file and replace it with the second half of the flag.
```
hacker@piping~appending-output:~$ /challenge/run >> /home/hacker/the-flag
.
.
.
[PASS] Success! You have satisfied all execution requirements.
I will write the flag in two parts to the file /home/hacker/the-flag! I'll do
.
.
get the whole flag!
hacker@piping~appending-output:~$ cat the-flag
pwn.college{4PaTtyUK-DiFvDHSfBIJN7JGPdg.QX3ATO0wiN3AzNzEzW}
```

## What I learned
Difference between using the '>' and the '>>'.
'>' completely replaces the file with whatever output we're redirecting.
'>>' adds the redirected output to the given target file.

## References 
reference material from pwn.college.
