# Detaching and attaching
in this challenge we will learn to detach and reattach our virtual terminal.

## My solve
**Flag:** `pwn.college{YMJ1Qk2pg55GK9aYOobKqWyPydR.0lN4IDOxwiN3AzNzEzW}`


```
screen
[CTRL A+D]
screen -r
150.pts-0.terminal-multiplexing~launching-screen (Remote or dead)
187.pts-2.terminal-multiplexing~detaching-and-attaching (Dead ???)
144.session_16a6fea3ab91be51 (Remote or dead) 135.challenge_session (Remote or dead)
.
.
.
139.pts-0.terminal-multiplexing~detaching-and-attaching
screen -r 139.pts-0.terminal-multiplexing~detaching-and-attaching
Here's your flag:
pwn.college{YMJ1Qk2pg55GK9aYOobKqWyPydR.0lN4IDOxwiN3AzNzEzW}
```

## What I learned
i can now detach and reattach screen.

## References 
reference material from pwn.college
