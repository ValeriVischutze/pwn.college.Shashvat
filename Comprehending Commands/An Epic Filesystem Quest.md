# An Epic Filesystem Quest
The aim of the challenge is to apply the various listing, changing directory and printing files commands to finally secure the flag.

## My solve
**Flag:** `pwn.college{E_f4UCn7VDklkDOsvE1oG--rMGz.QX5IDO0wiN3AzNzEzW}`

1)We changed directory to the root before utlizing the listing tool to obtain the POINTER file.
2) We open the file using the `cat` to open the file and use the listing /tool to access the subsequent file and obtain more clues before switching to that directory and repeating the process.
3) In certain clues, we are restricted from switching the directory or even having to access hidden files.
At the end of this cumbersome quest, we come across the `/usr/share/javascript/mathjax/unpacked/jax/output/SVG/fonts/Neo-Euler/Size4` file, listing which reveals a certain .GIST file. Upon opening it using the `cat` command we obtain the flag.

## What I learned
To apply the various commands learnt in the previous challenges and working upon the basics to level down onto the final flag.

## References 
Reference material from pwn.college
