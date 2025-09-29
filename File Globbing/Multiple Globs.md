# Multiple globs

We are supposed to run /challenge/run using multiple globs to cover all words that contain p.

**Flag:** `pwn.college{gTgGukn2nlkRWW0PHDI3_pgu26I.0lM3kjNxwiM0EzNzEzW}`

I changed my current directory to /challenge/files and then ran the program /challenge/run. we needed to convert all files that had the letter “p” somewhere within three characters. So, I used a pattern with “p” that matches any filenames starting and ending with "p" and having “p” in the middle as well.


```
hacker@globbing~multiple-globs:~$ cd /challenge/files/
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{gTgGukn2nlkRWW0PHDI3_pgu26I.0lM3kjNxwiM0EzNzEzW}
```

## What I learned

I learnt how to use multiple globs and how * can even represent nothing so you can make any pattern of your wishing or requirement

## References
none
