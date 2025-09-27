# Hidden Files

we need to find the hidden flag which hidden as a dot-prepended file in / directory.

**Flag:** `pwn.college{QwrC4SfFfemOhnKG_y9-1DPG7Ay.QXwUDO0wiM0EzNzEzW}`

I changed the current working directory to / using cd command then I used the ls command with the -a flag to see all the files including the ones which start with a '.' which are hidden. there si a file called '.flag-31613195598643' which can be acesssed using the cat command hence returning the required flag.
```
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv            bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-31613195598643  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-31613195598643
pwn.college{QwrC4SfFfemOhnKG_y9-1DPG7Ay.QXwUDO0wiM0EzNzEzW}
```

## What I learned

The ls command doesn't list all the files by default. it doesn't list the hidden files which start with '.' by default. We need to invoke ls with -a flag to view these hidden files. in this challenge we found the hidden flag using this same command and flag.

## References
NONE
