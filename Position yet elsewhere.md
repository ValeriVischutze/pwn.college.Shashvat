# Position yet elsewhere
The aim of the challenge, just like the two previous challenges, is to position ourselves in the given target directory and run the intended target command to obtain the flag

## My solve:
**Flag:** `pwn.college{ALPDZCx3RB1LYa4yE3y7kUo3ivA.QX4QTN0wiN3AzNzEzW} `

We first and foremost extract the conditions for the specified path for our challenge by positioning ourselves to the `/challenge` directory ( by using the `cd /challenge`) and extracting the contents of the `run` text file (using the `cat run` command).
This helps us obtain a set of candidate directories, one of which is intended to be the target.
Upon further 'browsing' and issuing the target command through these candidate directories, we rule out that the `/usr/bin` directory is the intended target directory and issuing the challebnge command:`/challenge/run` invokes the flag.
Invoking the target command in any other candidate directory issues a warning which also specifies the correct target directory and hence enables us to solve the challenge.

## What I learned:
To extract the challenge conditions from a given directory before browsing through the list of potential target directories and finding out the right target and issuing the intended target command.

## References:
Reference video from pwn.college
