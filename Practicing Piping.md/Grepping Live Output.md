# Grepping Live Output
This challenge asks me to grep for my flag in the outputs of /challenge/run.

## My solve
**Flag:** `pwn.college{UHGPoRvrnF9nYIpqG6anVPQ4AvP.QX5EDO0wiN2AzNzEzW}`

The outputs of /challenge/run are piped into the input of grep pwn.college using | which looks for the flag in the outputs of /challenge/run.
```bash
/challenge/run | grep pwn.college
```

## What I learned
Piping can be done by inserting | between the commands. Standard output from the command to the left of the pipe will be connected to (piped into) the standard input of the command to the right of the pipe. This  "cuts out the middleman" and avoids the need to store results to a file.

## References 
Resources and pretext in pwn.college
