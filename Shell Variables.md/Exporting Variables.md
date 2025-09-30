## Printing Variables
This challenge asks me to export PWN which is set to COLLEGE and the set COLLEGE to PWN and finally run /challenge/run.

## My Solve
**Flag:** 'pwn.college{YQRsPKzkE0QpotJ3mFKzCHC4IG8.QXyYTN0wiN2AzNzEzW}'

export PWN=COLLEGE can be given as a single command where both the tasks(assigning as well as exporting) are taking place. Then, PWN is assigned to COLLEGE without exporting. Finally, /challenge/run is run.
```
export PWN=COLLEGE
COLLEGE=PWN
/challenge/run
```

## What I Learned
Variables are exported to prevent leakage of sensitive data.

## References
Pretext
