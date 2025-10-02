# Translating Characters
This challenge asks me to run /challenge/run and then change the case of the flag provided.

## My Solve
**Flag:** 'pwn.college{kLH4QY9PRDsxFVsnao6tksNHuGY.01MxEzNxwiN2AzNzEzW}'

/challenge/run is executed by typin it on the command line. This prints : Your case-swapped flag:
PWN.COLLEGE{Klh4qy9prdSXfvSNAO6TKSnhUgy.01mXeZnXWIn2aZnZeZw}. This means I must use tr command to change the case. So all the letters from A-Z must change into a-z and vice versa. Hence, the following commands are given:
```
/challenge/run
echo PWN.COLLEGE{Klh4qy9prdSXfvSNAO6TKSnhUgy.01mXeZnXWIn2aZnZeZw}| tr A-Za-z a-zA-Z
```

## What I Learned
'tr' is a command used to change the case. It translates the character provided in its first argument to the character provided in its second argument. The command is given by: | tr arg_1 arg_2

## References
Pretext in pwn.college
