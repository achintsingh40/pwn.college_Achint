# home sweet home

In this challenge, /challenge/run will write a copy of the flag to any file you specify as an argument on the commandline, with these constraints:  
1. Your argument must be an absolute path.
2. The path must be inside your home directory.
3. Before expansion, your argument must be three characters or less. 

**Flag:** `pwn.college{AHYHrQgoLZbdSRmNPaEJPVE3okk.QXzMDO0wiM0EzNzEzW}`

In this challenge we need to write(copy) the flag to a file in the directory /home/hacker. 
'hacker@dojo:~$ /challenge/run YOUR_PATH_HERE' this is the way to specify the path. Out flag gets written in the ~/h. this is the way to mention file where we want to write the flag.      

```
hacker@paths~home-sweet-home:/tmp$ /challenge/run ~/h
Writing the file to /home/hacker/h!
... and reading it back to you:
pwn.college{AHYHrQgoLZbdSRmNPaEJPVE3okk.QXzMDO0wiM0EzNzEzW}
```
the tmp thing is not needed (was just figuring out something) 

## What I learned

How do we write comething in a file and understood that the expansion of ~ is an absolute path, and only the leading ~ is expanded. This means, for example, that ~/~ will be expanded to /home/hacker/~ rather than /home/hacker/home/hacker.

## References
none