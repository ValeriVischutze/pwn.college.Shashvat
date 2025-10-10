## Backgrounding processes
This challenge's run needs you to suspend it, then resume it. Good luck!

### Solve
**Flag:**  `pwn.college{4ctNqyB3Av-F7610xhjRDlz-b24.QX3QDO0wiN3AzNzEzW}`

We invoke  `/challenge/run` then sespended it using ctrl-Z and backgrounded it using bg commang launched another copy of `/challenge/run`.

```bash
/challenge/run

I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!
[1]+  Stopped                 /challenge/run
^Z
[1]+  Stopped                 /challenge/run

/challenge/run

I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!
.
.
.
I found a second version of me, but it's suspended! Please resume it in the
background with the 'bg' command, then run me again.

bg
[1]+ /challenge/run &

Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out.

/challenge/run

Yay, I found another version of me running in the background! Here is the flag:
pwn.college{4ctNqyB3Av-F7610xhjRDlz-b24.QX3QDO0wiN3AzNzEzW}
```

### What I learnt:
backgrounding a process using bg command.

### References:
Reference material from pwn.college
