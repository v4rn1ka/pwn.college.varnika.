# Multiple Globs
This challenge asks me to run /challenge/run with a single arguement that contains all the files which have the letter p in their name and are stored in /challenge/files.

## My solve
**Flag:** `pwn.college{oOVJuNXJqc2zPClfZpwxLoC7cLf.0lM3kjNxwiN2AzNzEzW}`

Using cd, I changed the cwd into /challenge/files and used * p * as the argument which includes all the files with the letter p.
```
cd /challenge/files
/challenge/run *p*
```

## What I learned
When * characters * is mentioned in the shell, then it looks for files that start with anything (including nothing) then have characters, and end in anything.

## References 
Pretext
