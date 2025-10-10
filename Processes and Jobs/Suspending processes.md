## Suspending processes
This level's run wants to see another copy of itself running and using the same terminal. How? Use the terminal to launch it, then suspend it, then launch another copy while the first is suspended!

### Solve
**Flag:**  `pwn.college{cFamF7buUojNqzY7ZZTCuHEUz7s.QX1QDO0wiN3AzNzEzW}`

We invoke `/challenge/run`ssssss then suspending it using ctrl-Z then running a copy of the same process.

```
/challenge/run

I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run

/challenge/run

I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

Yay, I found another version of me! Here is the flag:
`pwn.college{cFamF7buUojNqzY7ZZTCuHEUz7s.QX1QDO0wiN3AzNzEzW}`
```

### New Learnings
ctrl-Z can suspend a process to the backround.

### References:
Reference material from pwn.college
