# Matching With ?
This challenge asks me to change the directory to challenge, globbing c and l with ? and then executing run.

## My solve
**Flag:** `pwn.college{gctOtgZPxd1bGTZJYh4weRKtnjN.QXyIDO0wiN2AzNzEzW}'

The condition specifies, globbing must be used and the cd command would include the argument /?ha??enge. Once the directory is changed, thr run program can be executed.
```bash
cd /?ha??enge
./run
```

## What I learned
When '?' is found, the shell tries to replace the single character that match with the pattern.

## References 
Pretext
