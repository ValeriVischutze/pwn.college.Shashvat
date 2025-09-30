# Reading input
In this challenge, your job is to use read to set the PWN variable to the value COLLEGE.

## My solve
**Flag:** `pwn.college{gSp34yZZ9IPJ7wMAiviH9dR2aED.QX4cTN0wiN3AzNzEzW}`

```
read -p "INPUT: " PWN
INPUT: COLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{gSp34yZZ9IPJ7wMAiviH9dR2aED.QX4cTN0wiN3AzNzEzW}
```
In this challenge we used read to read the initial input and -p to get input as read -p "INPUT: " PWN.


## What I learned
To read command reads the data from my standard input and -p argument is used to get input into a variable.

## References 
Reference material from pwn.college
