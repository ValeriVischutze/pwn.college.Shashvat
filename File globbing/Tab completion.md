# Tab completion
Aim: this challenge has copied the flag into /challenge/pwncollege, and you can freely cat that file. But you can't type the filename: we used some serious trickery to make sure that you must tab-complete it. 

## My solve
**Flag:** `pwn.college{YmkbWTNMXwjBMDA3wxhL3WiHO3-.0FN0EzNxwiM5AzNzEzW}`


```
cat /cha<TAB>/pwnco<TAB>
pwn.college{YmkbWTNMXwjBMDA3wxhL3WiHO3-.0FN0EzNxwiM5AzNzEzW}
```
In this challenge we pressed tab after cha and after pwnco as cat /cha/pwnco.

## What I learned
Tab key can expand the name which we are writting.

## References 
Reference material from pwn.college
