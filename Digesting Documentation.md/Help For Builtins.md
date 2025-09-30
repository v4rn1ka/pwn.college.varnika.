# Help For Builtins
This challenge asks me to use help builtin to find my flag.

## My solve
**Flag:** `pwn.college{8YlkA0w6HarZOZdN65AyRozDQC8.QX0ETO0wiN2AzNzEzW}`

After I use the help builtin, it provides me additional argument with a secret code 8YlkA0w6 which when run all tother give me the flag.
```
help challenge
challenge --secret 8YlkA0w6
```

## What I learned
Some commands, rather than being programs with man pages and help options, are built into the shell itself. These are called builtins.

## References 
pretext
