## Process exit codes
In this challenge, you must retrieve the exit code returned by /challenge/get-code and then run /challenge/submit-code with that error code as an argument. Good luck!

### Solve
**Flag:** `pwn.college{QbbNUKKx78-GHNUbIxJJwcfjSGp.QX5YDO1wiN3AzNzEzW}`

run the /challenge/get-code and get the exit code by using ? variable and prepend it with $ as echo $? to read the exit code and then run the /challenge/submit-code with the exit code as /challenge/submit-code [EXIT_CODE] . 

```
/challenge/get-code
Exiting with an error code!

echo $?
85

/challenge/submit-code 85
CORRECT! Here is your flag:
pwn.college{QbbNUKKx78-GHNUbIxJJwcfjSGp.QX5YDO1wiN3AzNzEzW}
```

### What I learnt:
? variable. can be used to read the exit code of a program. And to read its value we have to prepend it with $.

### References:
Reference material from pwn.college
