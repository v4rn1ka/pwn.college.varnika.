# Sorting Data
This challenge asks me to sort thr flags present in /challenge/flags.txt in alphabetiical order to find the real flag at the end.

## My Solve
**Flag:** 'pwn.college{4WLfRmHZKi4BWAFuFDEUclI3yvP.0FM0MDOxwiN2AzNzEzW}'

In order to sort the data in the file in alphabetical order, we must give the sort command with the only argument being the file /challenge/flags.txt. This sorts all the flags present in it in alphabetical order and displays them. The real flag can then be retrieved as it is the last one. 
```
sort /challenge/flags.txt
```

## What I Learned 
The sort command helps the user organize data. It reads lines from input (or files) and outputs them in sorted order. By default, sort orders lines alphabetically. Arguments can change this:<br>
    -r: reverse order (Z to A) <br>
    -n: numeric sort (for numbers) <br>
    -u: unique lines only (remove duplicates) <br>
    -R: random order

## References
Pretext in pwn.college
