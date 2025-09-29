# Grepping Stored Results
This challenge asks me to redirect the output of /challenge/run into /tmp/data.txt ans then look for the flag in it.

## My solve
**Flag:** `pwn.college{ANzH2klJn4CL_mRg7wXgWUnKgbx.QX4EDO0wiN2AzNzEzW}`

The output of /challenge/run to is redirected /tmp/data.txt using > and then the grep command is used to look for the flag. 
```bash
/challenge/run > /tmp/data.txt
grep pwn.college /tmp/data.txt
```

## What I learned
Stored results can be grepped.

## References 
Pretext in pwn.college
