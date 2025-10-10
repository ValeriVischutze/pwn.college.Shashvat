## Resuming processes
This challenge's run needs you to suspend it, then resume it. Good luck!

### Solve
**Flag:** `pwn.college{kWNYpxK9HasHqbNNnxhnw4-0vHd.QX2QDO0wiN3AzNzEzW}`

suspending the process by pressing ctrl-Z and then resuming it using fg command.

```bash
/challenge/run

Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run

fg
/challenge/run
I'm back! Here's your flag:
pwn.college{kWNYpxK9HasHqbNNnxhnw4-0vHd.QX2QDO0wiN3AzNzEzW}
Don't forget to press Enter to quit me!

Goodbye!
```

### What I learnt:
`fg` command can be used to resume a suspended process.

### References:
Reference material from pwn.college
