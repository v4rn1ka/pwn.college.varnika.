# Extracting The First Lines With Head
This challenge asks me to pipe the first 7 lines of the output of /challenge/pwn into /challenge/college.

## My Solve
**Flag:** 'pwn.college{MIn0-jek9SmabC9siGPmqVQgw2p.0lNxEzNxwiN2AzNzEzW}'

To pipe the first 7 lines of /challenge/pwn, the head command along with the flag -n (to specify the number of lines) are used. Now these 7 lines of /challenge/pwn are piped into /challenge/college as required.
```
$ /challenge/pwn | head -n 7 | /challenge/college
```

## What I Learned
The head command is used to display the first few lines of its input. -n flag is added to specify the number of lines required. So th command is given as | head -n number-of_lines.

## References
Pretext
