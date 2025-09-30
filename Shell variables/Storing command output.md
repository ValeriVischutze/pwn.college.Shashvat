# Storing command output
Read the output of the /challenge/run command directly into a variable called PWN, and it will contain the flag!

## My solve
**Flag:** `pwn.college{w529tYTmAkclG_BjKB0UCAqIMW9.QX1cDN1wiN3AzNzEzW}`

```
PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
echo $PWN
pwn.college{w529tYTmAkclG_BjKB0UCAqIMW9.QX1cDN1wiN3AzNzEzW}
```


## What I learned
I can store the output of a command by setting it as a value to a variable

## References 
Reference material from pwn.college
