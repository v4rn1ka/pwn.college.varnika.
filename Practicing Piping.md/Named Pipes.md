# Named Pipes
This challenge asks me to create a named pipe /tmp/flag_fifo file and redirect the stdout of /challenge/run to it.

## My Flag
**Flag:** pwn.college{4TQjEWQPa0S9bOvxYpwEwggdUrt.01MzMDOxwiN2AzNzEzW}

/tmp/flag_fifo is created using mkfifo and then the contents of /challenge/run are redirected into the fifo. In order for this to run the fifo must be read as well. Hence, it gets catted. The order of reading and wriing doesn't matter while using fifos unlike files.
```
mkfifo /tmp/flag_fifo
cat /tmp/flag_fifo
/challenge/run > /tmp/flag_fifo
```

## What I learned
mkfifo is used to create a named pipe which is now called a fifo because we control them. One problem with FIFOs is that they'll block any operations on them until both the read side of the pipe and the write side of the pipe are ready. Therefore, two terminals are required, one for reading the file and the other for writing.

## References
Pre text in pwn.college
