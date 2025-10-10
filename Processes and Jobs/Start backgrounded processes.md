## Starting backgrounded processes
Now it's your turn to practice! Launch /challenge/run backgrounded for the flag!

### Solve
**Flag:** `pwn.college{UfOlKR6IuFu5RGMmPo2fybxa2Av.QX5QDO0wiN3AzNzEzW}`

running the `/challenge/run` in background by appending with & argument as `/challenge/run &`.

```
/challenge/run &
[1] 141

Yay, you started me in the background! Because of that, this text will probably
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{UfOlKR6IuFu5RGMmPo2fybxa2Av.QX5QDO0wiN3AzNzEzW}

[1]+  Done                    /challenge/run
```

### What I learnt:
can run a process in backround using & argument.

### References:
Reference material from pwn.college
