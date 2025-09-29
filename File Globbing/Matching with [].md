# Matching with []

We are supposed to change the directory to /challenge/files which contains some files. We are to run /challenge/run with all these files as arguments which can be shorted by using [].

**Flag:** `pwn.college{IkK6Fm2eS-AflGmFSy_Q0bZ_58Z.QXzIDO0wiM0EzNzEzW}`

I first changed the current working directory to /challenge/files. Then I executed '/challenge/run file_[bash]' which then runs the program with all the files_ ending with the letters b, a, s and h individually. This was asked of us and gives us the required flag.

```
hacker@globbing~matching-with-:~$ cd /challenge/files/
hacker@globbing~matching-with-:/challenge/files$ /challenge/files$ /challenge/run file_[bash]
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{IkK6Fm2eS-AflGmFSy_Q0bZ_58Z.QXzIDO0wiM0EzNzEzW}
```

## What I learned

I learned about file globbing with square brackets []. Unlike the question mark ? which matches any single character square brackets let you match only the characters listed inside them. 

## References

none