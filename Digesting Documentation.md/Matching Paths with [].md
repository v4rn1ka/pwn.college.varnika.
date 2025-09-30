# Matching Paths With []
This challenge asks me to use [] and run the command /challenge/run from its root directory with arguments file_b, file_a, file_s, and file_h which are in /challenge/files.

## My solve
**Flag:** `pwn.college{cAPghEn67oij6BHXiCgqFUUd3CJ.QX0IDO0wiN2AzNzEzW}`

Executed the program with a single argument containing the files. This is done usimg bracket glob: file_[bash] 
```
/challenge/run/challenge/files/file_[bash]
```

## What I learned
The bracket glob [] can be used to match some subset of potential characters, specified within the brackets.

## References 
Pretext
