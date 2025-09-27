# Learning Comple Usage
This challenge asks me to understand the document provided and invoke the commands accordingly.

## My Solve
**Flag:** `pwn.college{0Pbofh0Cu0M70n4mVb2cLVqj8H6.QX1ITO0wiN2AzNzEzW}`

The document provided asks me to invoke /challenge/challenge along with the argument --printfile. The argument to the --printfile argument is the path of the flag to read i.e. /flag.
```bash
/challenge/challenge --printfile /flag
```

## What I learned
I learned that a single command with an argument itself can still take many more arguments. An example of this is find has a -name argument, and the -name argument itself takes an argument specifying the name to search for. Not all commands but a certain of them can do this.

## References 
Pretext
