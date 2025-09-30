# Grepping Errors
This challenge asks me to find my flag in the errors of /challenge/run.

## My solve
**Flag:** `pwn.college{otIxhRelbqa3g7LwbGZqwbcYY0D.QX1ATO0wiN2AzNzEzW}`

Errors of /challenge/run are redirected to /challenge/run using 2 >& 1 and then this is piped to the command which finds the flag.
```bash
/challenge/run 2>&1 | grep pwn.college
```

## What I learned
The shell has a >& operator, which redirects a file descriptor to another file descriptor. Here, we redirect standard error to standard output (2>& 1) and then pipe the now-combined stderr and stdout as normal (|).

## References 
References and pretext in pwn.college
