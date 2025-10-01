# Position Yet Elsewhere
This challenge asks me to change my directory to the one that is provided and then invoking the path of the run file.

## My Solve
**Flag:** 'pwn.college{g8NmAcLOEaS1sm8SLQdFZ25lPCd.QX4QTN0wiN2AzNzEzW}'

First I provided the path of the run file: /challenge/run. Then it mentioned that I had to change the directory to /proc/131. So, I added the command cd /proc/131 which changed it to the var directory. After this I could rerun the challenge program and got my flag.
```
cd /proc/131
/challenge/run
```

## What I Learned
I learnt that the 'cd' command is used to change the'current working directory'. 
The command is give by cd /directory.

## References
Video in pwn.college
