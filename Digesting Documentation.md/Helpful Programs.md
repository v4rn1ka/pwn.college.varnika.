# Helpful Programs
This challenge asks me to find the flag by practicing --help.

## My solve
**Flag:** ` pwn.college{seLt7LqyFtjVVuVR97OKf_TC3qt.QX3IDO0wiN2AzNzEzW}`

The first time I use --help, it gave me a list of other arguments. Using -p, i recieved a secret code 797 which when added to -g gave me the flag.
```
/challenge/challenge --help
/challenge/challenge -p
/challenge/challenge -g 797
```

## What I learned
Some programs don't have a man page, but might tell you how to run them if invoked with a special argument like --help.

## References 
pretext
