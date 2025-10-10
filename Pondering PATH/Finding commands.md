# Finding commands
In this challenge, we added a win command somewhere in your $PATH, but it won't give you the flag.
Instead, it's in the same directory as a flag file that we made readable by you! You must find win (with the which command), and cat the flag out of that directory.

## My solve
**Flag:** `pwn.college{4U-ms0NItxaZnAJaHvymc6JKTMc.01NzEzNxwiN3AzNzEzW}`

```
which win
/challenge/paths/17072/win 
cd /challenge/paths/17072
cat flag
pwn.college{4U-ms0NItxaZnAJaHvymc6JKTMc.01NzEzNxwiN3AzNzEzW}
```

## What I learned
I can now find commands using `which` command

## References 
Reference material from pwn.college
