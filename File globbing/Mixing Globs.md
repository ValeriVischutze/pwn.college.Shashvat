# Mixing globs
cd to /challenge/files and using the globbing you've learned, write a single, short (6 characters or less) glob that (when passed as an argument to /challenge/run) will match the files "challenging", "educational", and "pwning"!

## My solve
**Flag:** `pwn.college{Qhr1G5_2xASPKkOBaYbtjOv7UEh.QX1IDO0wiN3AzNzEzW}`


```
cd /challenge/files
/challenge/run [cep]*
You got it! Here is your flag!
pwn.college{Qhr1G5_2xASPKkOBaYbtjOv7UEh.QX1IDO0wiN3AzNzEzW}  
```
In this challenge we run the /challenge/run with [cep]* argument as c,e,p are the first letter of the file names thats why its inside the [] glob.

## What I learned
mixed globs for argument.

## References 
Reference material from pwn.college
