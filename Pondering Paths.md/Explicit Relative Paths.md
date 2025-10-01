# Explicit Relative Paths, from /
This challenge asks me to use '.' in the relative path to run /challege/run

## My Solve
**Flag:** 'pwn.college{0MGED8DxHrxyVJW9JaY0UfHjbrz.QXwUTN0wiN2AzNzEzW}'

First, I changed the directory to the root directory. Then, the explicit relative path would be ./challenge/run. Here, '.' implies that the rest of the path relates to the current working directory that is the root directory in this case.
```
 cd /
./challenge/run
```

## What I learned
The only difference between implicit and explicit relative directories is that in implicit it is assumed that the path relates to the cwd while in explicit it is necessary to mention its source using '.' (signifying current directory) or '..' (signifying the directory that the cwd lives in). 

## References
Video and slides in pwn.college
