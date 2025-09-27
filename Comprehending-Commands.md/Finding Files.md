# Finding Files
This challenge asks me to find the flag which is hidden in a random directory.

## My solve
**Flag:** `pwn.college{QHtdqEoi1xPPN3e3vcB33C6_W1x.QXyMDO0wiN2AzNzEzW}`

```
find / -name flag
cat /usr/local/lib/python3.8/dist-packages/pytz/zoneinfo/Africa/flag
```
After using the find command, there appeared many paths. So, I used cat to read each of them and find my flag.

## What I learned
find is a command used to find files. They can be given by find or be specific like find / -name file_name.

## References 
pretext
