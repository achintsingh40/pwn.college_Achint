
# Reading Manuals

We have to read the manual for challenge to understand how to obtain the flag.

**Flag:** ` pwn.college{8L5Na62dd0TZWWhYhLxsUKFc-qd.QX0EDO0wiM0EzNzEzW}`

I ran 'man challenge' command to get the manual page for challenge. On the man page, three options were given out of which only  --addhhx NUM gave hint to the flag. It said that 856 instead of NUM would give us the flag. Looking at the syntax in the man page, I entered '//challenge/challenge --addhhx 856' which gave me the required flag.
```
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --addhhx 856
Correct usage! Your flag: pwn.college{8L5Na62dd0TZWWhYhLxsUKFc-qd.QX0EDO0wiM0EzNzEzW}
```

## What I learned

I learnt about man pages which are built-in documentations for commands and programs. They help us get information about a command or program without needing to access the internet. I also learnt how to read a man page about a specific command and understand what to use from the man page to obtain the required flag.

## References
none