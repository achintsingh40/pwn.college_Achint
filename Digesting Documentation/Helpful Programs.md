# Helpful programmes


The challenege asks us to read the documentation of a program using --help instead of man pages to obtain the way to get the flag.


**Flag:** `pwn.college{0GAnOm9ZuK0T0uoGsnBUFhlU0QZ.QX3IDO0wiM0EzNzEzW}`

I used the --help option in the program /challenge/challenge to see its instructions. The help showed an option called -g, which would print a special number needed to get the flag. After finding this number, which was 90, I ran the program with /challenge/challenge -g 753  and it gave the flag


```
hacker@man~helpful-programs:~$  /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$  /challenge/challenge -p
The secret value is: 90
hacker@man~helpful-programs:~$ /challenge/challenge -g 90
Correct usage! Your flag: pwn.college{0GAnOm9ZuK0T0uoGsnBUFhlU0QZ.QX3IDO0wiM0EzNzEzW}
```

## What I learned

I Learnt  alternative ways to read the documentation of a program with --help, -h, -?, help or even /

## References

none