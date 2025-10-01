# Writing to multiple programs.
In this challenge, we have /challenge/hack, /challenge/the, and /challenge/planet. Run the /challenge/hack command, and duplicate its output as input to both the /challenge/the and the /challenge/planet commands!

## My solve
**Flag:** `pwn.college{09yG6BfNIqnC6B_CPMDQyv1tbsU.QXwgDN1wiN3AzNzEzW}`

In this challenge, we duplicate the output of /challenge/hack to /challenge/the and /challenge/planet as /challenge/hack | tee >(/challenge/the) | /challenge/planet .
```
/challenge/hack | tee >(/challenge/the) | /challenge/planet
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{09yG6BfNIqnC6B_CPMDQyv1tbsU.QXwgDN1wiN3AzNzEzW}
```

## What I learned
learnt to copy data using >().

## References 
Reference material from pwn.college
