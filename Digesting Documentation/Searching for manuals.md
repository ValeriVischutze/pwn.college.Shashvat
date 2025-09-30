# Searching for manuals
Find the hidden manpage and read it to get the flag.

## My solve
**Flag:** ` pwn.college{wYCcmWHaBLAIzsDEmbwnV_fxxSB.QX2EDO0wiN3AzNzEzW}`


```
man -k challenge
wcmazsmbwn (1)       - print the flag!
man wcmazsmbwn
/challenge/challenge --wcmazs 203
Correct usage! Your flag: pwn.college{wYCcmWHaBLAIzsDEmbwnV_fxxSB.QX2EDO0wiN3AzNzEzW}
```
First we read the man man manpage in which we came across about apopros then used it to search for challenge manpage using man -k challenge then read the challenge manpage followed instruction , got the flag.

## What I learned
man -k apropos search tool ,Search the short manual page descriptions for keywords and display any matches.

## References 
Reference material from pwn.college
