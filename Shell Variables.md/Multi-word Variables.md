## Printing Variables
This challenge asks me to assign the variable PWN the value COLLEGE YEAH.

## My Solve
**Flag:** 'pwn.college{oYW90LDYONNBt9ueg3Szal4jWn6.QXwYTN0wiN2AzNzEzW}'

While assigning multiple values for a single variable, the avlues are put in "..." so that the shell understands that they are to be assinged to the same variable. It would run everything after a space as a command if the double quotes aren't used. Here, COLLEGE YEAH are to be assigned to PWN hence, they are enclosed in double quotes. 
```
PWN="COLLEGE YEAH"
```

## What I Learned
Assigning multiple values to a single variable can be done by using double quotes.

## References
Pretext
