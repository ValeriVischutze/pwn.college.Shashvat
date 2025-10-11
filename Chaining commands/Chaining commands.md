# Chaining with semicolons
Give it a try now! In this level, you must run /challenge/pwn and then /challenge/college, chaining them with a semicolon.
Solve

**Flag:**  `pwn.college{Uzr4sCG1q3j_mmjkKXnLqCAIURL.QX1UDO0wiM5AzNzEzW}`

chaining /challenge/pwn and /challenge/college with semi-colon as /challenge/pwn ; /challenge/college

```
/challenge/pwn ; /challenge/college
Yes! You chained /challenge/pwn and /challenge/college! Here is your flag:
pwn.college{Uzr4sCG1q3j_mmjkKXnLqCAIURL.QX1UDO0wiM5AzNzEzW}
```

## What I learnt:
chaining two commands into a single line using semi-colon.



# Building on Success
In this challenge, you need to chain the programs /challenge/first-success and /challenge/second using the && operator.
Solve

**Flag:** pwn.college{wB-qG3CO06R10-SdINS_q2YVNyN.0lM0MDOxwiM5AzNzEzW}

chaining /challenge/first-success and /challenge/second using && as /challenge/first-success && /challenge/second
```
/challenge/first-success
/challenge/second

Error: /challenge/first-success must be successfully chained with
/challenge/second using &&

/challenge/first-success && /challenge/second

Nice chaining! Flag: pwn.college{wB-qG3CO06R10-SdINS_q2YVNyN.0lM0MDOxwiM5AzNzEzW}
```

## What I learnt:
chaining programs using && operator . second program will only run when the first program executes successfully.
Handling failure


# Handling Failure
In this challenge, you need to chain /challenge/first-failure and /challenge/second using the || operator. Go for it!
Solve

**Flag:**  pwn.college{4dbOK4ZWc79hvjTEXCjN-GzMO5o.01M0MDOxwiM5AzNzEzW}

chained the /challenge/first-failure with /challenge/second as /challenge/first-failure || /challenge/second

```
/challenge/first-failure || /challenge/second
Nice chaining! Flag: pwn.college{4dbOK4ZWc79hvjTEXCjN-GzMO5o.01M0MDOxwiM5AzNzEzW}

New Learnings

chaining two programs with || operator works only if the first command fails.


Your first shell script

Same as last level, run /challenge/pwn and then /challenge/college, but this time in a shell script called x.sh, then run it with bash!
Solve




**Flag:** pwn.college{80hosJtNrC3Fzho_jVjoHNC7kUT.QXxcDO0wiM5AzNzEzW}

echo "/challenge/pwn; /challenge/college" > x.sh
bash x.sh
Great job, you've written your first shell script! Here is the flag:
pwn.college{80hosJtNrC3Fzho_jVjoHNC7kUT.QXxcDO0wiM5AzNzEzW}
```

## What I learnt:
i can now develop shell scripts.



# Redirecting script output

In this level, we will practice piping (|) from your script to another program. Like before, you need to create a script that calls the /challenge/pwn command followed by the /challenge/college command, and pipe the output of the script into a single invocation of the /challenge/solve command!
Solve

**Flag:** pwn.college{QceAAogf6SYPWdbGrBaJ8F8O6Xo.QX4ETO0wiM5AzNzEzW}

```
echo "/challenge/pwn; /challenge/college" > x.sh
bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{QceAAogf6SYPWdbGrBaJ8F8O6Xo.QX4ETO0wiM5AzNzEzW}
```

## What I learnt:
I can now use piping to redirect outputs of a script to another command.




# Executable shell scripts
Make a shellscript that will invoke /challenge/solve, make it executable, and run it without explicitly invoking bash

## My solve
**Flag:** `pwn.college{033y_OrJtGmEBTBZ3dDn1PWBnnQ.QX0cjM1wiM5AzNzEzW}`

```
echo "/challenge/solve" > flag.sh
chmod  +x flag.sh
./flag.sh
Congratulations on your shell script execution! Your flag:
pwn.college{033y_OrJtGmEBTBZ3dDn1PWBnnQ.QX0cjM1wiM5AzNzEzW}
```

## What I learnt:
I can now run shell scripts as executables without the need of bash.




# Scripting with Arguments
For this challenge, you need to write a script at /home/hacker/solve.sh that:

    Takes two arguments
    Outputs them in REVERSE order (second argument first, then the first argument)


## My solve

**Flag:** `pwn.college{QjXO1H1YigN0HrbZ2z94raNaulv.0VNzMDOxwCNAzNzEzW}`

```
cat > /home/hacker/solve.sh <<'EOF'
>echo "$2 $1"
>EOF
chmod +x /home/hacker/solve.sh
/home/hacker/solve.sh pwn college
/challenge/run
Here's your flag:
pwn.college{QjXO1H1YigN0HrbZ2z94raNaulv.0VNzMDOxwCNAzNzEzW}
```

## What I learnt:
Learnt how to reverse a given order.



# Scripting with conditionals
For this challenge, write a script at /home/hacker/solve.sh that:

    Takes one argument
    If the argument is "pwn", output "college"
    For any other input, output nothing


## My solve:
**Flag:** `pwn.college{cga_kLppsc0BGqFALn_5WitkWRp.0lNzMDOxwCN3AzNzEzW}`

```
cat >/home/hacker/solve.sh <<'EOF'
>if["$1"="pwn"]
then
echo "college"
fi
EOF
chmod +x /home/hacker/solve.sh
/home/hacker/solve.sh pwncollege
/home/hacker/solve.sh foo
/challenge/run
Here's your flag:
pwn.college{cga_kLppsc0BGqFALn_5WitkWRp.0lNzMDOxwCN3AzNzEzW}
```

## What I learnt:
I can now script with given conditionals.




# Scripting with default cases
Once your script works correctly, run /challenge/run to get your flag!

## My solve:
**Flag:** `pwn.college{cfpPG1IQJsSNAVZa6NrTjYYohOG.01NzMDOxwCN3MDM0EzW}`

```
cat > /home/hacker/solve.sh <<'EOF'
if ["$1"=="pwn"]
then
echo "college"
else
echo "nope"
fi
EOF
chmod +x /home/hacker/solve.sh
/challenge/run
Here's your flag:
pwn.college{cfpPG1IQJsSNAVZa6NrTjYYohOG.01NzMDOxwCN3MDM0EzW}
```

## What I learnt:
learnt to incorporate conditional statements with scripting.



# Scripting with Multiple conditions
For this challenge, write a script at /home/hacker/solve.sh that:

    Takes one argument
    If the argument is "pwn", output "college"
    For any other input, output "nope"
Once your script works correctly, run /challenge/run to get your flag!


## My solve:
**Flag:** `pwn.college{kkx30e4QSm0Rb2FaRywXN9_AEkT.0FOzMDOxwCN3MDM0EzW}`

```
cat > /home/hacker/solve.sh <<'EOF'
if["1"=="hack"]
then
echo "the planet"
elif["1"=="pwn"]
then
echo "college"
elif["1"=="learn"]
then
echo "linux"
else
echo "unknown"
fi
EOF
chmod +x /home/hacker/solve.sh
/challenge/run
Here's your flag:
pwn.college{kkx30e4QSm0Rb2FaRywXN9_AEkT.0FOzMDOxwCN3MDM0EzW}
```

## What I learnt:
Incorporating multiple conditional statements




# Reading shell scripts
In this level, we will learn to read shell scripts. /challenge/run is a shell script that requires you to put in a secret password, but that password is hardcoded into the script iself! Read the script (using, say, cat), figure out the password, and get the flag!


## My solve:
**Flag:** `pwn.college{UEhHxSQ6fZ0rWIOUu6INq8uNPhA.0lMwgDOxwCN3AzNzEzW}`


```
/challenge/run
hack the PLANET
CORRECT! Here's your flag:
pwn.college{UEhHxSQ6fZ0rWIOUu6INq8uNPhA.0lMwgDOxwCN3AzNzEzW}
```

## What I learnt
Passwords incorporated into the shell script.
