# Extracting Specific Sections Of Text
This challenge asks me to extract the flag from /challenge/run which contains random numbers and single characters as columns.

## My Solve
**Flag:** 'pwn.college{w0kQYziirX7Ac6dtjH5ZFGt7kvT.01NxEzNxwiN2AzNzEzW}'

It is mentioned that the singe characters(flag) is the second column in the data stored in /challenge/run. Hence, it must be extracted using the cut command along with the space being the delimiter and 2 being the feild number. In order to bring it into the flag format in one line, the new lines (\n) must be removed using trace. Combiniing these we get our final command:
```
/challenge/run | cut -d " " -f 2 | tr -d '\n'
```

## What I Learned
Cut command is used to draw specific columns of data. The -d argument specifies the column delimiter (how columns are separated). In this case, it's a space character. The -f argument specifies the field number (which column to extract). So, the total command is written as cut -d ' ' -f column_required.

## References
Pretext
