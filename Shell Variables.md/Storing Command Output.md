# Storing Command Output
This challenge asks me to store the command /challenge/run which contains the flag in the variable PWN.

## My Solve
**Flag:** 'pwn.college{ksgk0MrPNaSz033Y7A6GZmydSDo.QX1cDN1wiN2AzNzEzW}'

The output of command /challenge/run is stored in the variable PWN and then it is printed using echo.
```
PWN=$(/challenge/run)
echo $PWN
```

## What I Learned
Command substitution allows the output of a command to replace the command itself. The standard form of command substitution occurs when a command is enclosed as $(command).

## References
Pretext and resurces in pwn.college
