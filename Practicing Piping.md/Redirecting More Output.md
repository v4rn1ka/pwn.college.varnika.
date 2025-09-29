# Redirecting More Output
This challenge asks me to uredirect the output of /challenge/run to myflag. 

## My solve
**Flag:** `pwn.college{IXCE1bGNCEE-H5i--0Z8NgkZMgM.QX1YTN0wiN2AzNzEzW}`

Using > symbol redirects the output of /challenge/run to myflag. Then, the output can be viewed by catting myflag. 
```bash
/challenge/run > myflag
cat myflag
```

## What I learned
Aside from redirecting the output of echo, we can redirect the output of any command as well. This is done using the same symbol.

## References 
Resources and pretext in pwn.college
