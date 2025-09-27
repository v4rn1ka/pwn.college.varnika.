# Exclusionary Globbing
This challenge asks me to run /challenge/run with all files in /challenge/files that don't start with p, w, or n.

## My solve
**Flag:** `pwn.college{MRls3mPLAo_fKvt5MsLIW0nW_ry.QX2IDO0wiN2AzNzEzW}`

Change the directory to where the files are present: /challenge/files. Then, [] is used because we have three letters(3 cases), ! because a negation is required, * because we must explude al the words starting with the specified letters. 
```
 cd /challenge/files
/challenge/run [!pwn]*
```

## What I learned
! is used inside breackets to invert the glob and the bracket instance matches characters that aren't listed. 

## References 
Pretext
