# Exporting variables
The aim of the challenge In this challenge, we have to invoke /challenge/run with the PWN variable exported and set to the value COLLEGE, and the COLLEGE variable set to the value PWN but not exported (e.g., not inherited by /challenge/run). 

## My solve
**Flag:** `pwn.college{wA52zuRpFb2OXN43VwkE3xWuLq_.QXyYTN0wiN3AzNzEzW}`

```
COLLEGE=PWN
You've set the COLLEGE variable to the proper value!

PWN=COLLEGE
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!

export PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!

/challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{wA52zuRpFb2OXN43VwkE3xWuLq_.QXyYTN0wiN3AzNzEzW}
```
In this challenge set value PWN to variable COLLEGE then set value COLLEGE to variable PWN export PWN then run /challenge/run to invoke the flag.

## What I learned
To export command , minimize shell implementation that is invoked as a child of the main shell process.

## References 
Reference material from pwn.college
