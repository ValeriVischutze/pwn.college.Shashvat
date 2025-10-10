## Detaching and Attaching (tmux)
tmux (terminal multiplexer) is screen's younger, more modern cousin. It does all the same things but with some different key bindings. The biggest difference? Instead of Ctrl-A, tmux uses Ctrl-B as its command prefix.

### Solve
**Flag:** ` pwn.college{gZRl5HYKOx9-epwpe4t835ke_Sn.0VO4IDOxwiN3AzNzEzW}`

```bash
tmux
[CTRL+B, d]
/challenge/run
tmux a
Congratulations, here is your flag:  pwn.college{gZRl5HYKOx9-epwpe4t835ke_Sn.0VO4IDOxwiN3AzNzEzW}
```

### What I learnt:
learning to detach/reattach in `tmux`

### References:
Reference material from pwn.college
