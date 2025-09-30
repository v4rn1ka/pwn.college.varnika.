# Writing To Multiple Programs
This challenge asks me to copy the stdout of /challenge/hack to the stdins of boththe commands /challenge/the as well as /challenge/planet.

## My solve
**Flag:** `pwn.college{o5mmtEF6T9d810oEB945nG9k_Ao.QXwgDN1wiN2AzNzEzW}`

 tee creates temperoroy named pipes for both the commands and then the output of /challenge/hack is piped to both of these commands.
```bash
/challenge/hack | tee >(/challenge/the) >(/challenge/planet)
```

## What I learned
Output can be duplicated from one command to multiple commands. This can be done by combining tee , process substitution and piping. First process substitution is used to create temperory files for the commands. Then, tee assumes them to be files and duplicates the output of the inital commands into these temperory files. 

## References 
Pretext in pwn.college
