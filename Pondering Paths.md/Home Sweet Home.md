# 9. Home Sweet Home
This challenge ask me to specify a file within /challenge/run as an argument on the commandline with the constraints: 
i.Argument must be an absolute path
ii. The path must be inside the home directory
iii. Before expansion, argument must be 3 characters or less.

## My Solve
**Flag:** 'pwn.college{0BWgfnJsusJif4iIn-CJXK0xzAg.QXzMDO0wiN2AzNzEzW}'

Considering the first 2 constraints, I came to the conclusion that the arguement must begin with ~/. Here, ~ is the home directory. These add up to 2 characters, which means I can add only one more character. Let that be v. This completes my argument (~/v). 
```
/challenge/run ~/v
```

## What I learned
~ is the home directory which expands to /home/hacker.

## References
Pre text from the challenge.
