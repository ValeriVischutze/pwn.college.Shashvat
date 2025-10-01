# Duplicating piped data with tee
The aim of the challenge is to intercept the data of the /challenge/pwn being piped into /challenge/college.

## My solve
**Flag:** `pwn.college{wCoAH3V8rhXukh3WwsRhb06qmJp.QXxITO0wiN3AzNzEzW}`

 Here we  passed `/challenge/pwn | tee flag | /challenge/college` then  invoked `cat /flag` that gave me SECRET_ARG for `/challenge/pwn` then used it in the correct way to get flag. 
 Finally we invoke `/challenge/pwn --secret "wCoAH3V8" | tee flag | /challenge/college` to obtain the flag.
```
/challenge/pwn | tee flag | /challenge/college

Processing...
WARNING: you are overwriting file flag with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be

cat flag

Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "wCoAH3V8"

/challenge/pwn --secret "wCoAH3V8" | tee flag | /challenge/college 

Processing...
WARNING: you are overwriting file flag with tee's output...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{wCoAH3V8rhXukh3WwsRhb06qmJp.QXxITO0wiN3AzNzEzW}
```

## What I learned
How to intercept data

## References 
Reference material from pwn.college
