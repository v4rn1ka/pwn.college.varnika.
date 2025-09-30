# Filtering With grep -v
This challenge asks me to filter out the DECOY flags from the standard outputs of /challenge/run.

## My Solve
**Flag:* 'pwn.college{ssYa414PxfkMSMBKu0Ck4vy1FK2.0FOxEzNxwiN2AzNzEzW}'

grep -v filters out the DECOY flags from the stdout of /challenge/run and displays the required flag. 
```
 /challenge/run | grep -v DECOY
```

## What I Learned
grep -v shows lines that do NOT match a pattern and is used in filtering out content. 

## Rferences
Resources and pretext in pwn.college
