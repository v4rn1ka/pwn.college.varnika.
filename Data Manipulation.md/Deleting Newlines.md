# Deleting Newline
This challenge asks me to delete the unnecessary spaces and lines from the flag present in /challenge.run.

## My Solve
**Flag:**  'pwn.college{YmWamlMljv4FUPXJsh_Y5hN2Grc.0VNxEzNxwiN2AzNzEzW}'

Path to the flag is first given, and then tr command with -d flag is used to delete "\n", basically new lines from the flag stored in /challenge/run.
```
$/challenge/run | tr -d "\n"
```

## What I Learned
The backslash (\) signifies that the character that follows it is a standin for a character that's hard to input into the shell normally. In case we actually want to refer to the character '\' then, '\\' is to be used.

## Reference
Pretext
