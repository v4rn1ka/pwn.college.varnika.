# Symbolic Links
This challenge asks me to use symlink to recieve my flag from /challenge/catflag. It is given that challenge/catflag will read out home/hacker/not-the-flag while the flag is stored in /flag.

## My Solve
**Flag:** 'pwn.college{soJMcYyr6x2ARJcbB4Vnt1LFhu5.QX5ETN1wiN2AzNzEzW}'

I begin with creating a symbolic link (home/hacker/not-the-flag) of /flag. Now, when I run the command /challenge/catflag, the flag is received because /challenge/catflag reads home/hacker/not-the-flag which is now a symlink of /flag.
```
ln -s /flag /home/hacker/not-the-flag
/challenge/catflag
```
## What I Learned
Soft links store the path to a particular file and not the contents of the file. Hence, when the original file is deleted, it's soft link becomes unaffective.

Hard links store the data of the original file. Hence, remain unaffected upon modifying the original file.

## References
Video and slides in pwn.college
