# Redirecting Errors
This challenge asks me to redirect the output of /challenge/run to myflag and its errors to instructions. 

## My solve
**Flag:** `pwn.college{glSOryI_aBknkummmhm2BF54ao7.QX0YTN0wiN2AzNzEzW}`

The output of /challenge/run is redirected to myflag using > and the errors using 2>. Later, the flag is retrieved using cat command. Catting instructions would provide the errors.
```
/challenge/run > myflag 2> instructions
cat myflag
```

## What I learned
A File Descriptor (FD) is a number that describes a communication channel in Linux.<br>
    FD 0: Standard Input<br>
    FD 1: Standard Output<br>
    FD 2: Standard Error<br>
We must redirect process communication using FD numbers. > implies FD 1 or 1>.

## References 
Resources in pwn.college
