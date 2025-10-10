# Changing Permissions
in this challenge we will learn about changing file permissions.

## My solve
**Flag:** `pwn.college{g3AvNR43_zC1ia3xDbJO70hbx-8.QXzcjM1wiM5AzNzEzW}`


```
cd /
cat flag
cat: flag: Permission denied
ls -l flag
-r-------- 1 root root 60 Oct 10 18:27 flag
chmod a+r
cat flag
pwn.college{g3AvNR43_zC1ia3xDbJO70hbx-8.QXzcjM1wiM5AzNzEzW}
```

## What I learned
I can now change file permissions.

## References 
Reference material from pwn.college
