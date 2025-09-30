# Duplicating Piped Data with tee
This challenge asks me to pipe /challenge/pwn into /challenge/college while intercepting the data to see what pwn needs.

## My solve
**Flag:** `pwn.college{Q6Iy82HbnIXMDy17PE2LEePXe17.QXxITO0wiN2AzNzEzW}`

tee command first duplicates /challenge/pwn into pwn_output. Then, pwn_output is read using the cat command. It provides a secret argument to be added i.e. --secret Q6Iy82Hb. Once this is added to the original command, the flag is printed.
```bash
/challenge/pwn | tee pwn_output | /challenge/college
cat pwn_output
/challenge/pwn --secret Q6Iy82Hb | /challenge/college
```

## What I learned
The tee command duplicates data flowing through your pipes to any number of files provided on the command line.

## References 
Pretext of the challenge.
