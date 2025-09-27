# Matching With *
This challenge asks me to change the directory to challenge but not using more than 4 characters in the cd command and then /challenge/run.

## My solve
**Flag:** `pwn.college{M2Jfl19ljYjgMRd6n6VYQpeleXt.QXxIDO0wiN2AzNzEzW}`

The condition specifies no more than 4 characters so globbing must be used and the cd command would include the argument /ch*. Once the directory is changed, thr run program can be executed.
```bash
cd /ch*
./run
```

## What I learned
Globbing is used to reference files without typing them all out, or typing out their full paths. When '*' is found, it tries to replace arguments that match with the pattern.

## References 
Pretext
