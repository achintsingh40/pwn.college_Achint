# Challenge Name

The challenge asks us to create two blank files pwn and college in the tmp directory using the touch command, after which we run /challenge/run to get the flag.

**Flag:** `pwn.college{oKSr4JXDgPx6_ucvExFZfBE35E3.QXwMDO0wiM0EzNzEzW}`

I directly created the files using touch <absolute path of the file> as given in the question. then run the /challenge/run command and ogt the flag.

```
hacker@commands~touching-files:~$ touch /tmp/pwn
hacker@commands~touching-files:~$ touch /tmp/college
hacker@commands~touching-files:~$ /challenge/run
Success! Here is your flag:
pwn.college{oKSr4JXDgPx6_ucvExFZfBE35E3.QXwMDO0wiM0EzNzEzW}
```

## What I learned

i learnt how to create files using touch command 

## References

none
