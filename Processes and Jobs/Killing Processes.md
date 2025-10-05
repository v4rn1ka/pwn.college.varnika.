# Killing Processes
This challenge asks me to kill the /challenge/dont_run to run /challenge/run.

## My Solve:
**Flag:** 'pwn.college{o1vbskvCNHgOpwCpaJiE9Uc0PG6.QXyQDO0wiN2AzNzEzW}'

Begin with printing the processes using ps -ef. Now, look for /challenge/dont_run and take a note of its PID. Next, kill this process using the command kill and argument PID. After killing it, /challenge/run can be executed.
```
ps -ef
kill 136
/challenge/run
```

## What I Learned
Processes can be killed using the kill command. The argument of this command must  be th PID of the process to be killed.

## References
Pretext
