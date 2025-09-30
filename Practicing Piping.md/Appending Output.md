# Redirecting Output
This challenge asks me to append the out of /challenge/run to /home/hacker/the-flag. 

## My solve
**Flag:** `pwn.college{8c_WWLAK_VjMS3VS68cDpMrepBR.QX3ATO0wiN2AzNzEzW}`

Appending uses the symbol >> and add the contents of /challenge/run to /home/hacker/the-flag. The output(flag) can then be printed using cat command. 
```bash
/challenge/run >> /home/hacker/the-flag
cat /home/hacker/the-flag
```

## What I learned
'>>' is used when we do not want to truncate the file instead add the output to the file.

## References 
Resources in pwn.college
