# Switching windows (tmux)
We've created a tmux session with two windows:

    Window 0 has the flag!
    Window 1 has your warm welcome.

Go get that flag!


## My solve
**Flag:** `pwn.college{0pbaI5xCSHykjs0Z-gpfSs5NE8V.0FM5IDOxwiN3AzNzEzW}`


```
tmux ls
challenge_session: 2 windows
tmux attach -t challenge_session
[Ctrl-B 0]
Excellent work! You found window 0!
Here's your flag:
pwn.college{0pbaI5xCSHykjs0Z-gpfSs5NE8V.0FM5IDOxwiN3AzNzEzW}
```

## What I learned
I can now navigate and manage windows using tmux (terminal multiplexer).

## References 
Reference material from pwn.college
