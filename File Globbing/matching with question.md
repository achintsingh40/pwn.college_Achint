# Matching with ?

Change the directory to /challenge using ? instead of the letters c and l. Then we have to run /challenge/run to get the flag.

**Flag:** `pwn.college{helloworld}`

I replaced c and l with ? in the argument to cd to change the directory and then ran /challenge/run to obtain the required flag.
 
 ```
This challenge resets your working directory to /home/hacker unless you change
directory properly...
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /?ha??enge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{86Xq3BPymErCM0mwU46eXiB_Omf.QXyIDO0wiM0EzNzEzW}
```

## What I learned

I learnt about ? which functions the same way as * but only replaces single characters and not all patterns like *.

## References
none