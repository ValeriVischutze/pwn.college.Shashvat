# Cat:not the pet but the command
The aim of the challenge is to familiarize with the `cat` command.

## My solve:
**Flag:** `pwn.college{gPGt6pkksevKzuX54X6tV0ZZVfA.QXxcTN0wiN3AzNzEzW} `

The `cat` commands enables us to display a text file. The overall syntax for this command is `cat argument.txt`.
If no arguments are assigned it'll automatically display the user input in the terminal, which is essentially null. If any arguments are assigned like for instance, `cat wassupfolks`, it'll simply print `wassupfolks` as the output
For the given challenge, the flag was attached in the text file called `flag` which was stored in the home directory. To obtain the flag, we simply outputted the text file by using `cat flag`

## What I learned:
The function of cat as a reader for text files or user text displayer.

## References:
Reference material from pwn.college challenge
