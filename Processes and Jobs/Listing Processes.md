# Listing Processes
This challenge asks me to find the flag which is stored in /challenge/run which is now renamed. ls option is not available therefore, ps -ef or ps aux is to be used.

## My Solve
**Flag:** 'pwn.college{Q4hl0_fepSuldH2FtjJ8IUPc2Bw.QX4MDO0wiN2AzNzEzW}'

The only way to find the required file is by printing all the processes running on the terminal. This would eventually print the file as well. This can be done using ps command along with the arguments -es or aux. An additional ww is added to the arguments to avoid truncation. Once, the command is give, a list of processes appear out of which /challenge/10975-run-13037 is likely to be the most suitable file. Hence, on running this, the flag gets printed. 
```
 ps -efww
 /challenge/10975-run-13037
```

## What I Learned
ps is used to print all the ongoing processes on the terminal.There are two ways to specify arguments of ps:<br>

"Standard" Syntax: -e can be used to list "every" process and -f for a "full format" output, including arguments. These can be combined into a single argument -ef.<br>
"BSD" Syntax: a can be used to list processes for all users, x to list processes that aren't running in a terminal, and u for a "user-readable" output. These can be combined into a single argument aux.<br>

Both display the user (USER column), the PID, the TTY, the start time of the process (STIME/START), the total utilized CPU time (TIME), and the command (CMD/COMMAND). ps -ef additionally outputs the Parent Process ID (PPID), while ps aux outputs the percentage of total system CPU and Memory that the process is utilizing. 

## References
Pretext
