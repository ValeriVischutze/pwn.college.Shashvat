# Multiple options for Tab completeion
This challenge has a /challenge/files directory with a bunch of files starting with pwncollege. Tab-complete from /challenge/files/p or so, and make your way to the flag!

## My solve
**Flag:** `

```
/challenge/files/pwn<f1><TAB><TAB>
pwn                    pwncollege-family      pwncollege-flyswatter
pwn-college            pwncollege-flag        pwncollege-hacking
pwn-the-planet         pwncollege-flamingo
cat /challenge/files/pwncollege-flag

```

## What I learned
Using f1 key and then pressing tab key 2nd time prints all the files under that particular directory.

## References 
Reference material from pwn.college
