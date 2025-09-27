# Hidden Files
This challenge asks me to find my flah which is hidden in a dot pretend file in /.

## My solve
**Flag:** `pwn.college{UtlXaBgfOh9r_GMKW-aNuw987vz.QXwUDO0wiN2AzNzEzW}`

First, changed the directory to / using cd command and then, used ls -a command to list all the files including the hidden ones. There existed a file .flag.... Finally, I used the cat command to read this file.
```
cd /
ls -a
cat .flag-26440149524697
```

## What I learned
ls -a is a command used to list the files hideen. Files are usually hidden when ther start with a dot.

## References 
pretext
