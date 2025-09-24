# Implicit relative paths, form /
In this challenge we are asked to use a realtive paths (which does not start with '/)  . 

## My Solve
**Flag:** 'pwn.college{QzumplRNYAsAZAJVs-tRu8fnAbn.QX5QTN0wiM0EzNzEzW}'

First we change the directory using 'cd /', now our directory is '/' . now we run challenge/run using the relative path while having current directory of '/' .  
```
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{QzumplRNYAsAZAJVs-tRu8fnAbn.QX5QTN0wiM0EzNzEzW}
```

## What I Learned
i learnt how to run a challenge using a relative path and understood what realtive path actually means. 

## References
None.