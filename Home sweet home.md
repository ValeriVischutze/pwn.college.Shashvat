# Home sweet home
The aim of this challenge was to create a copy of the flag in the home directory

## My solve:
**Flag** `pwn.college{AwW1sGj7C-jZiY09pkC2CAT0X8X.QXzMDO0wiN3AzNzEzW} `

As always by default we start with the home directory.
To create a copy of the flag and store it in the home directory under the given constraints, we run the command `/challenge/run ~/t` , where `~/t`(home directory can be simply represented by `~`and hence we reduce the characters to match the constraint instead of home/hacker/t) is the argument equal to 3 characters and absolute path that is taken.
Bash copies the flag and saves it in the home directory, which is also printed back. It can also be accessed in the home directory by using the command `cat t`

## What I learned:
The significance of using `~` to represent the `/home/hacker`, which ultimately reduces the no. of characters (atleast according to one of the constraints in our challenge). Also, `~/~` would be expanded as `home/hacker/~`.

## References:
Reference material of the challenge
