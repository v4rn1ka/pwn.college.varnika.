# Tab Completion
This challenge asks me to use the tab key to complete the file name instead of *

## My solve
**Flag:** `pwn.college{4BP1bVC8RRZlq9WldJuFRSAkKpv.0FN0EzNxwiN2AzNzEzW}`

The flag was stored in /challenge/pwncollege and so I clicked on the tab key instead of enter to complete the file name. 
```
cat /challenge/pwn<TAB>}
```

## What I learned
The tab key is much safer that the * while completing the file names as * glob might expand to unintentional files.

## References 
Pretext
