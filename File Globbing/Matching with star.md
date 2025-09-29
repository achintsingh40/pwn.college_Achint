# Matching with *

We have to change the current working directory to /challenge using * and not using more than four characters as argument to cd and then run /challenge/run.

**Flag:** `pwn.college{owz6VCoPuKC5Pip019kWCQOuteI.QXxIDO0wiM0EzNzEzW}`
I first typed cd /c*/ where /c*/ uses a wildcard and counts as four characters for the cd command. This changed my current directory to /challenge. Using the same idea with * as a wildcard, I was then able to run the program /challenge/run.
```
This challenge resets your working directory to /home/hacker unless you change
directory properly...
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /c*/
hacker@globbing~matching-with-:/challenge$ /c*/r*
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{owz6VCoPuKC5Pip019kWCQOuteI.QXxIDO0wiM0EzNzEzW}
```

## What I learned

I learned about globbing, which is a way to shorten how we write file paths by using wildcards. The * symbol is a wildcard that matches any pattern before the command runs. The * matches any part of the filename except for / or a leading.

## References

none