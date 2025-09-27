# Comparing Files

### We have 2 files in 2 diff directories. one has al fake flags and other one has 1 real flag and both have a huge number of flags. We need to use the diff command and find the real flag.
    

**Flag:** `pwn.college{Q6b3X3-5gLFv7J57gbO4tHUt2H_.01MwMDOxwiM0EzNzEzW}`

We've been given that one file contains a 100 fake flags and the other contains a 100 fake flags plus the real flag under the challenge directory.  The diff function is used to find the difference between two files and the difference would be the flag. 

```
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
35a36
> pwn.college{Q6b3X3-5gLFv7J57gbO4tHUt2H_.01MwMDOxwiM0EzNzEzW}
```

## What I learned

the diff command is used to find the difference between the contents of 2 files  

## References
none