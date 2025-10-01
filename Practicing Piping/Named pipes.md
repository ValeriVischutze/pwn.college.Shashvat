# Named Pipes
 The aim is to create a /tmp/flag_fifo file and redirect the stdout of /challenge/run to it. Once successful, /challenge/run will write the flag into the FIFO

## My solve
**Flag:** `pwn.college{02db9nEMfBZljEBf4iiaIv2aix7.01MzMDOxwiN3AzNzEzW}`

In this challenge, we first create a FIFO at the the given target directory. We then use the cat command to print out the data.
Upon switching to terminal-2, we pipe the stdout of /challenge/run to /tmp/flag_fifo before invoking the cat command once more.
Upon doing so, we obtain the flag in terminal-1
```
In terminal-1:
mfifo /tmp/flag_fifo
cat /tmp/flag_fifo

In terminal-2:
/challenge/run > /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo
.
.
.
cat/tmp/flag_fifo

In terminal-1:
You've correctly redirected /challenge/run's stdout to a FIFO at
/tmp/flag_fifo! Here's your flag:
pwn.college{02db9nEMfBZljEBf4iiaIv2aix7.01MzMDOxwiN3AzNzEzW}
```

## What I learned
How to create and control a FIFO.

## References 
Reference material from pwn.college
