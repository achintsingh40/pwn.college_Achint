# Searching for manuals

Wehave to go through the man page for man and find the appropriate command to search for the name of the manual which will help us get the flag.

**Flag:** `pwn.college{Yd_qpXgIAQxUJJLR7bFM8sgA9DA.QX2EDO0wiM0EzNzEzW}`

After reviewing the manpage for man, I discovered the -k  keyword option, which when ran with flag man -k flag. This command revealed a manual entry for dqpgxbsgwi, which provided instructions for getting the flag . searching in dqpgxbsgwi manpage I found the argument  --dqpgxb NUM, and by passing the value 789, I obtained the flag.



```
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k challenge
dqpgxbsgwi (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man dqpgxbsgwi
hacker@man~searching-for-manuals:~$ /challenge/challenge  --dqpgxb 789
Correct usage! Your flag: pwn.college{Yd_qpXgIAQxUJJLR7bFM8sgA9DA.QX2EDO0wiM0EzNzEzW}
hacker@man~searching-for-manuals:~$
```

## What I learned

I learnt how the man page for man can be used to find the man page for the needed command if the man page is not known.
## References

none