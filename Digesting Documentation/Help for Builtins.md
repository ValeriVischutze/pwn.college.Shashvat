# Help for Builtins
This challenge's challenge command is a shell builtin, rather than a program. Like before, you need to lookup its help to figure out the secret value to pass to it!

## My solve
**Flag:** `pwn.college{wYxvcSwL5h7e7c68nEaaEaNkOIX.QX0ETO0wiN3AzNzEzW}`


```
help challenge
 You must be sure to provide the right value to --secret. That value
 is "wYxvcSwL".
challenge --fortune
challenge --version
I'm exactly the version I need to be!
challenge --secret wYxvcSwL
correct! Here is your flag!
pwn.college{wYxvcSwL5h7e7c68nEaaEaNkOIX.QX0ETO0wiN3AzNzEzW}
```
Upon carefully browsing through the results of `help challenge`, we come across the secret value to the prompt `--secret`, issuing which invokes the flag.

## What I learned
Builtin command help gives a list of shell builtins by running the builtin help. We can procure assistance on a specific command using builtin help

## References 
Reference material from pwn.college
