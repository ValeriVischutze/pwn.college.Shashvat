# Reading files
Read /challenge/read_me into the PWN environment variable, and we'll give you the flag! The /challenge/read_me will keep changing, so you'll need to read it right into the PWN variable with one command!

## My solve
**Flag:** `pwn.college{ET0dTPGpfYFInBokIAgtIP9zZT4.QXwIDO0wiN3AzNzEzW}`

```
read "PWN" < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{ET0dTPGpfYFInBokIAgtIP9zZT4.QXwIDO0wiN3AzNzEzW}
```
In this challenge,we read the file /challenge/read_me using < as read "PWN" < /challenge/read_me.

## What I learned
To read from the file using < .

## References 
Reference material from pwn.college
