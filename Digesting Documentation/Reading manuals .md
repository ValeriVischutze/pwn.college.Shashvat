# Reading manuals
The aim of the challenge to obtain the flag by invoking the given target command under a specific argument which can be deduced by using the `man` command

## My solve:
**Flag:** `pwn.college{sBqQcxelt-iSsbazjhp3k8vooJS.QX0EDO0wiN3AzNzEzW} `

```
hacker@man~reading-manuals:~$ cd /challenge
hacker@man~reading-manuals:/challenge$ man challenge
hacker@man~reading-manuals:/challenge$ /challenge/challenge --fortune
No stopping or standing.
hacker@man~reading-manuals:/challenge$ /challenge/challenge --version
I'm exactly the version I need to be!
hacker@man~reading-manuals:/challenge$ /challenge/challenge --sqcxel 380
Correct usage! Your flag: pwn.college{sBqQcxelt-iSsbazjhp3k8vooJS.QX0EDO0wiN3AzNzEzW} 
```
The `man` command enables us to view the 'manual' of a given command. We can scroll up and down by using the respective arrow keys or quit by clicking on `q`.
The given description upon invoking `man challenge` allowed us to deduce that the triggering command `/challenge/challenge` must be followed up by the argument `--sqxcel 380` in order to obtain the flag.
```
DESCRIPTION  
          Output the flag when called with the right arguments.

    --fortune
        read a fortune
    
    --version
         output version information and exit

     --sqcxel NUM
           print the flag if NUM is 380
```



## What I learned:
How to apply the `man` command to deduce the challenge conditions before applying the same.

## References 
Reference material from pwn.college
