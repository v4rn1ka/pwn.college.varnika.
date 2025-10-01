# Mixing Globs
This challenge asks me to write a glob (6 characters or less) that (when passed as an argument to /challenge/run) will match the files "challenging", "educational", and "pwning".

## My solve
**Flag:** `pwn.college{oUiR8WjKY2gD2_dYjQewcyDiS8x.QX1IDO0wiN2AzNzEzW}`

Using cd, I changed the cwd into /challenge/files and then used [cep]* as the glob as it includes all the combinations of words beginning with c,e,p/
```
cd /challenge/files
/challenge/run [cep]*
```

## What I learned
I learnt to mix globs.

## References 
Pretext
