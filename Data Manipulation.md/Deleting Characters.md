# Deleting Characters
This challenge asks me to delete the additionally added characters(^,%) using tr.

## My Solve:
**Flag:** 'pwn.college{0PYZgEnf5j2EBWc3Oudn3H66ElW.0FNxEzNxwiN2AzNzEzW}'

First, I run /challenge/run and it printed my character stuffed flag. In order to remove the characters(^,%) , I needed to use tr -d command along with with the characters to be removed,^,%.
```
/challenge/run
echo p%w%n%.^c%o^l^%l^e^%g%e^{%0^%P%Y^Z^%g^E^%n^f^%5^%j^%2^%E^B^%W%c^3O^u^%d^%n^%3%H^
%6%6^%E^%l%W%.^%0^%F^%Nx^EzN%x^w^%i^N^2%A^z^%N%z^%E^%z^%W^%}^^ | tr -d ^%
```

## What I Learned
tr translates the character provided in its first argument to the character provided in its second argument

## References
Pretext in pwn.college
