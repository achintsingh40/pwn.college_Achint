# More Catting Practice

in this we read the flag file but from a different directory and not the home directory without using the cd command  

**Flag:** `pwn.college{QyXh4mRQiwbE2K8k0nATPgP9Dxy.QXwITO0wiM0EzNzEzW}`

in this we need to access the file from a different directory. the directory and its absolute is mentioned at the top of the the terminal. we write cat and the whole path of it and we can read the flag   

```
hacker@commands~more-catting-practice:~$ cat /lib/llvm-10/bin/flag
pwn.college{QyXh4mRQiwbE2K8k0nATPgP9Dxy.QXwITO0wiM0EzNzEzW}
```

## What I learned

how to read a file form a different directory without using the cd command. 

## References
none