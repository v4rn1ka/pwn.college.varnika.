# Redirecting Output
This challenge asks me to use this output redirection to write the word PWN to the filename COLLEGE. 

## My solve
**Flag:** `pwn.college{glSOryI_aBknkummmhm2BF54ao7.QX0YTN0wiN2AzNzEzW}`

Starting with echo PWN, the output of this command is PWN. > symbol is used to redirect the output to the mentioned file which is COLLEGE in this case. 
```bash
echo PWN > COLLEGE
cat COLLEGE
```

## What I learned
The > (left caret) symbol is used to redirect to a file. A single left caret will truncate the file, then enter the redirected data into the file; this effectively replaces your data. If the designated file does not exist the file will be created.

The > symbol will redirect stdout by default but you can specify whether to redirect stdout or stderr by putting the appropriate file descriptor in front of the redirect symbol.

## References 
Resources in pwn.college
