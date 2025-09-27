# making driectories
we are required to create a /tmp/pwn directory and make a file college in it. We then run /challenge/run to check our solution and it gives us the flag.

**Flag:** `pwn.college{gkDLtnlYu4Ou-LtPzxFRO0rbc1C.QXxMDO0wiM0EzNzEzW}`

I created the tmp/pwn directory in the home directory using mkdir command and changed the current working directory to it using cd. then i created a file named college using the touch command and then run the /challenge/run to check the program and it gave the flag.

```
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{gkDLtnlYu4Ou-LtPzxFRO0rbc1C.QXxMDO0wiM0EzNzEzW}
```

## What I learned

I learnt how to create a directory and make a file in it  

## References

none