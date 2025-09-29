# Redirecting Input
This challenge asks me to redirect PWN file into /challenge/run. PWN file contains the value COLLEGE.

## My solve
**Flag:** `pwn.college{Ykh_Yc07GvXfneQchmWrzVsoTv_.QXwcTN0wiN2AzNzEzW}`

First, store COLLEGE in PWN. This is done by redirecting the output of echo COLLEGE (which is COLLEGE) into PWN file. The input PWN is further redirected into /challenge/run.  
```bash
echo COLLEGE > PWN
cat PWN
/challenge/run < PWN
```

## What I learned
I learn that input can also be redirected using < symbol. 

## References 
Resources in pwn.college
