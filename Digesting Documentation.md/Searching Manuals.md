# Searching Manuals
The challenge asks me to search the challenge manual for the hint to print the flag.

## My solve
**Flag:** `pwn.college{kR881L2m4MwqNi8Tek5usTnHknh.QX1EDO0wiN2AzNzEzW}`

First, the command to read the manual. i.e man challenge. Then, use / for finding flag. n,N helped me switch between results. The hint was to use --lew as an argument. When it was used, the flag showed up.
```bash
man challenge
/flag
n
n
/challenge/challenge --lew
```

## What I learned
We can scroll man pages with the arrow keys (and PgUp/PgDn) and search with /. After searching, we can use n or N to go to the next or previous result respectively. Instead of /, we can use ? to search backwards.

## References 
Pretext.
