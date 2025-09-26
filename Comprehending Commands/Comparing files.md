# Comparing files
The aim of the challenge is to familiarize ourselves with comparing the contents of any two given files.

## My solve:
**Flag:** `pwn.college{0YAnEv58ZZ902LJbaH262Gh8nUz.01MwMDOxwiN3AzNzEzW} `

According to our problem, one file:`/challenge/decoys_only.txt` contained 100 fake flags and `/challenge/decoys_and_real.txt` contained those same 100 fake flags and one true flag. This means that comparing the two of them will enable us to obtain the true flag.
  we simply use the `diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt` to obtain the true flag.

## What I learned:
To compare any two given files. In this challenge, bash prints `20a21 `, which essentially means that the 20th line of file 1 was being changed with 21st line for file 2, which was essentially the difference between the two files.

## References:
Add any references or videos you used while solving the challenge.
