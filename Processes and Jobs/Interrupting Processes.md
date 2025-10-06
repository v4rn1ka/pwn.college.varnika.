# Interrupting Processes
This challenge asks me to interrupt /challenge/run to get my flag.

## My Solve
**Flag:** 'pwn.college{wN6VooIO-P4B5dEGtE0os2BfotR.QXzQDO0wiN2AzNzEzW}'

The first step is running /challenge/run. This leads to a text which asks me to interrupt the process. This is done using Ctrl+C. Once this is done, the flag is produced. 
```
/challenge/run
^C
```

## What I Learned
To interrupt a process, Ctrl+C is used.

## References
Pretext
