# Fun with group names
in this challenge we will check the group name using `id` and then change group ownership to the required group

## My solve
**Flag:** `pwn.college{UnFjjkrvRXlGzQZ56t1CmxSeaah.QXycjM1wiN3AzNzEzW} `

```
cd /
cat flag
cat: flag: Permission denied
id
uid=1000(hacker) gid=1000(grp28448) groups=1000(grp12850)
chgrp grp12850 flag
cat flag
pwn.college{UnFjjkrvRXlGzQZ56t1CmxSeaah.QXycjM1wiN3AzNzEzW} 
```

## What I learned
proficiency in using `id` and `chgrp`

## References 
Reference material from pwn.college
