# Process Substitution For Input
This challenge asks me to retrieve my flag from theoutputs of /challenge/print_decoys and /challenge/print_decoys_and_flag

## My solve
**Flag:** ` pwn.college{IfYzNHjy6JZm1uwq8288SxjauL0.0lNwMDOxwiN2AzNzEzW}`

The outputs of /challenge/print_decoys and /challenge/print_decoys_and_flag are compared and the non-common content is printed. 
```bash
diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
```

## What I learned
We can hook input and output of programs to arguments of commands. This is done using Process Substitution. <br>
When input process substitution, <(command) is used, it will run the command and hook up its output to a temporary file that it will create called the named pipe. 

## References 
Pretext in pwn.college
