# Implicit Relative Path
This challenge asks me to explicitly execute a program in the current directory, using '.'.

## My Solve
**Flag:** 'pwn.college{4Y3h5O4kI7IB40tLnhOg3Q4Ml_0.QXxUTN0wiN2AzNzEzW}'

Initially I changed the directory to /challenge and then explicitely run the run program with ./run.
```
 cd /challenge --> for changing the cwd to challenge
./run --> (.) implying to run it from the cwd
```

## What I learned
Using naked path could be unsafe as it might accidentally execute programs from the current directory which have the same name as the core system utilities. Using '.' makes it much safer.

## References
Pre-text from the challenge, slides in pwn.college.
