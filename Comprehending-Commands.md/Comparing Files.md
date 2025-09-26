# Comparing Files
This challenge asks me to find the flag which is the only different flag present in two given files.

## My solve
**Flag:** `pwn.college{8Qr416m0n6gmAIVCcHMk_jWJlgD.01MwMDOxwiN2AzNzEzW}`

It is mentioned that the one of the two given files contain the flag which means that the only difference between the two files is the flag. Hence, all i need to do is use the diff command and get my flag.
```
diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
```

## What I learned
diff is a command used to find the differnce between two files and display it. 

## References 
pretext
