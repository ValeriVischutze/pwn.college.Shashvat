# Finding sessions
in this challenge we will learn to detach/reattach to a particular screen if many screen sessions are running

## My solve
**Flag:** `pwn.college{Ie6BsEK9eJkSOzXVqR15H1soQVF.01N4IDOxwiN3AzNzEzW}`

```
screen -ls
screen -r session_d3309a58de2db4c3
.
.
.
pwn.college{Ie6BsEK9eJkSOzXVqR15H1soQVF.01N4IDOxwiN3AzNzEzW}
```

## What I learned
i can now navigate through multiple screen sessions.

## References 
reference material from pwn.college
