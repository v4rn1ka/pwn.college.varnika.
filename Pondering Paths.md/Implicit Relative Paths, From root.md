#  Implicit Relative Paths, from /
This challenge asks me to run /challenge/run using a relative path while having a current working directory of /.

## My Solve
**Flag:** 'pwn.college{0MGED8DxHrxyVJW9JaY0UfHjbrz.QXwUTN0wiN2AzNzEzW}'

Since it is mentioned that the cwd is the root directory, the implicit relative path would be the rest of it i.e. challenge/run. First, I changed the directory to the root directory and then I gave the relative path and got my flag.
```
cd /
challenge/run
```

## What I Learned
I learned how relative paths are dependent on the current working directory and that implicit relative path need not mention the current working directory. 

## References
Video and slides in pwn.college
