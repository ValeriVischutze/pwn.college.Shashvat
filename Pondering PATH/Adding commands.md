# Adding commands
in this challenge we will learn to make a shell script and add its location to the PATH

## My solve
**Flag:** `pwn.college{8N9HOaRYQ5iflYpJVwMCMmB7GNy.QX2cjM1wiN3AzNzEzW}`

```
mkdir /tmp/mybin
cat > /tmp/mybin/win <<'EOF'
/bin/cat /flag
EOF
chmod +x /tmp/mybin/win
export PATH=/tmp/mybin
/challenge/run
Invoking 'win'....
pwn.college{8N9HOaRYQ5iflYpJVwMCMmB7GNy.QX2cjM1wiN3AzNzEzW}
```

## What I learned
i can now make shell scripts, add it to PATH to invoke commands.


## References 
Reference material from pwn.college
