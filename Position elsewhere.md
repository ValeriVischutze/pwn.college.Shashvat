# Position elsewhere
The aim of the challenge is position ourselves in a given target directory and invoke the target command as per the conditions issued in the challenge directory.

## My solve:
**Flag:** `pwn.college{AwAd53ugt941RO7UokFxLZzwc2f.QX3QTN0wiN3AzNzEzW} `

Just like the previous challenge, we switch to the challenge directory (by using the `cd /challenge` command), obtain the list of candidate directories by getting the outputs of the `DESCRIPTION.md run` file (using the `cat run`).
We browse through the different candidate directories and find out that `/tmp` directory is the target directory and issuing the intended `/challenge/run` target command invokes the flag.
Running the command in any other directory will issue a `Incorrect...you're not currently in the /tmp directory`, which will easily let the user know that they were positioned in the wrong directory, if they issued the target command in any other directory.

## What I learned:
To extract the conditions for finding the suitable challenge directory and positioning myself in that directory to execute the challenge command.

## References:
Reference video from pwn.college
