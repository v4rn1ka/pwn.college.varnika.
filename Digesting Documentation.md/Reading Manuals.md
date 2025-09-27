# Reading Manuals
This challenge asks me to read the manual of challenge and print the flag according to the secret option.

## My solve
**Flag:** `pwn.college{UaGXD2ZxcGyFiajwYyhH1c6G6x8.QX0EDO0wiN2AzNzEzW}`

The manual can be read using the man command. The secret option in the manual suggests that adding the argument axcyia "216" to /challenge/challenge would print my flag. So, I invoked the command and got my flag.
```bash
man challenge
/challenge/challeneg --axcyia "216"
```

## What I learned
man is the short form of manual and is a command used to read the manuals of commands.It is given by man command_name(path not included). The manual mainly consists the name, synopsis and description of the command.

## References 
Pretext
