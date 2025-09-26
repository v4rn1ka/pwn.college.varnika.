# Challenge Name
This challenge asks me to create two new files (/tmp/pwn, /tmp/college) using touch and to execute /challenege/run.

## My solve
**Flag:** `pwn.college{o0ruaaWUATn0khOaJ_RdxPiNfPq.QXwMDO0wiN2AzNzEzW}`

Since, the path of both my new files contain tmp, I first changed the directory to /tmp using cd command. Then I created the two new files using the touch command followed by running /challenge/run.
```
cd /tmp
touch pwn
touch college
/challenge/run
```

## What I learned
touch is a command used to create new files. 

## References 
pretext
