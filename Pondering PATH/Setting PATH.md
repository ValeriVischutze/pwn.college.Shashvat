# Setting PATH
in this level's /challenge/run will run the win command via its bare name, but this command exists in the /challenge/more_commands/ directory, which is not initially in the PATH. 
The win command is the only thing that /challenge/run needs, so you can just overwrite PATH with that one directory.

## My solve
**Flag:** `pwn.college{EUlPkYl85m-EAh0xHRHc4vzxK3j.QX1cjM1wiN3AzNzEzW}`


```
cd /
export PATH=/challenge/more_commands/[CTRL+A, D]
/challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{EUlPkYl85m-EAh0xHRHc4vzxK3j.QX1cjM1wiN3AzNzEzW}
```

## What I learned
I can now set PATH to different directories

## References 
Reference material from pwn.college
