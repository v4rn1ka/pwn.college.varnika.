# Searching For Manuals
This challenge asks me to find the flag by following hints through man man.

## My solve
**Flag:** `pwn.college{wANlfZYo3GU5ihPQzx-D_52UVGj.QX2EDO0wiN2AzNzEzW}`

After opening man man, man -k suggested something about printing. Following that, i recieved a code (wlfoihzxjw) which when used opened another manual. This gave me the command along with the agrument.
```
man man
man -k challenge
man wlfoihzxjw
/challenge/challenge  --wlfoih 355
```

## What I learned
familiarised myself with manuals

## References 
pretext
