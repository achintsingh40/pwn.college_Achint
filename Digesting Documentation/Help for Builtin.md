# Help for Builtins

We are using help to look for information on the challenge builtin and then use relevant arguments to obtain the flag.

**Flag:** `pwn.college{M-za_8NrCmmHwuVOlUyxrEZbHIR.QX0ETO0wiM0EzNzEzW}`

I first Executed help on the challenge builtin to get info about challenge 'help challenge'. It gave me option from which one was  to obtain the flag which required a secret value and gave the secret value as well. So, on running ' challenge --secret M-za_8Nr' I got the required flag.

```
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "M-za_8Nr".
hacker@man~help-for-builtins:~$ /challenge --secret M-za_8Nr
bash: /challenge: Is a directory
hacker@man~help-for-builtins:~$ challenge --secret M-za_8Nr
Correct! Here is your flag!
pwn.college{M-za_8NrCmmHwuVOlUyxrEZbHIR.QX0ETO0wiM0EzNzEzW}
```

## What I learned

I  learn that built-in commands are special commands inside the shell itself and don’t exist as separate files. These built-in commands don’t have normal man pages like other commands, so we use the help command to see their manual. If you type help alone, it shows all built-in commands the shell supports. To see details about a specific built-in command type help followed by the command name.

## References

none