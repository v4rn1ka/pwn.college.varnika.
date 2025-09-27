# Matching With []
This challenge asks me to use [] and run the command /challenge/run with arguments file_b, file_a, file_s, and file_h which are in /challenge/files.

## My solve
**Flag:** `pwn.college{gLmye9fAM3NSkaCatW2jI8Y9LSp.QXzIDO0wiN2AzNzEzW}`

Using cd, I changed the cwd into /challenge/files and then executing run program a single argument containing the files. This is done usimg bracket glob: file_[bash] 
```
cd /challenge/files
/challenge/run file_[bash]
```

## What I learned
The bracket glob [] can be used to match some subset of potential characters, specified within the brackets.

## References 
Pretext
