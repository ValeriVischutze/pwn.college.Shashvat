# Linking files
use a symlink to read /flag via /challenge/catflag

## My solve
**Flag:** `pwn.college{434xRtR4_NVrCZtJlr5_Ib5yqbg.QX5ETN1wiN3AzNzEzW}`

```
rm /home/hacker/not-the-flag
ln -s /flag /home/hacker/not-the-flag
/challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{434xRtR4_NVrCZtJlr5_Ib5yqbg.QX5ETN1wiN3AzNzEzW}
```
Here, we first delete the stored file in /home/hacker/not-the-flag, then create a symlink for /flag in /home/hacker/not-the-flag, so that the /catflag programs reads the flag instead.

## What I learned
Learnt to create new symlinks.

## References 
Reference material from pwn.college
