# Multiple Options For Tab Completion
This challenge asks me to fetch my flag by looking /challenge/files directory which has multiple files starting with pwncollege.

## My Solve
**Flag:** 'pwn.college{0Y7QlKEgwAC-vjDS4DzTD7ufUy8.0lN0EzNxwiN2AzNzEzW}'

Begin with changing the directory to /challenge/files. Since the flag starts with pwn, try /challenge/files/pwn with tab completion. This diaplays a bunch of files out of which pwn-college seemed the closest to the flag. Upon trying tab completion with /challenge/files/pwn-college, more files are displayed out of which pwncollege-flag seemed the most accurate. Hence, upon catting that file, I recieved my flag.
```
cd /challenge/files
/challenge/files/pwn <TAB><TAB>
/challenge/files/pwn-college <TAB><TAB>
cat /challenge/files/pwncollege-flag
```

## What I Learned
Clicking on tab once, completes the file name whereas clicking twice, prints all the files. 

## References
Pretext 
