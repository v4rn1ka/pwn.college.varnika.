# Challenge Name
This challenge asks me to create a new file called delete_me, then delete it and finally execute /challenge/check.

## My solve
**Flag:** `pwn.college{oT5T7MnpCEVWFVT2KLfqP2YZpvW.QX2kDM1wiN2AzNzEzW}`

I started with creating delete_me using the touch command and then deleting it using rm followed by running /challenge/run.
```
touch delete_me
ls
rm delete_me
ls
/challenge/check
```

## What I learned
rm is a command used to delete existing files from a directory. This is done by giving the command rm file_to_be_deleted.

## References 
pretext
