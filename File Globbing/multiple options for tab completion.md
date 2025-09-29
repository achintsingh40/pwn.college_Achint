# multiple options for tab completion

This challenge has a /challenge/files directory with a bunch of files starting with pwncollege. We have to tab-complete from /challenge/files/p to reach the flag.

**Flag:** `pwn.college{Uzmziyk-9yJoKSIBpa1zG21cJoe.0lN0EzNxwiM0EzNzEzW}`

I typed cat /challenge/files/p and pressed Tab, which auto-completed it to pwn. Pressing Tab again showed possible options to expand. Then, by typing pwnc and pressing Tab, it auto-completed to pwncollege. Pressing Tab once more displayed options, and I finally completed the command to pwncollege-flag to get the flag.

```
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn
pwn                    pwn-the-planet         pwncollege-flag        pwncollege-flyswatter  
pwn-college            pwncollege-family      pwncollege-flamingo    pwncollege-hacking     
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-flag
pwn.college{Uzmziyk-9yJoKSIBpa1zG21cJoe.0lN0EzNxwiM0EzNzEzW}
```

## What I learned

Learnt how to see all the possible available options for tab completion.

## References

none