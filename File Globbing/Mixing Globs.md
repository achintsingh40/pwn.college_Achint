# Mixing Globs

We are given diversely-named files in /challenge/files and we are to run /challenge/run. We are supposed to glob such that we cover all arguments matching files "challenging", "educational", and "pwning".

**Flag:** `pwn.college{8DP7rwva5KhP0IX9Zc7d_lTx891.QX1IDO0wiM0EzNzEzW}`

I changed the current working directory to /challenge/files. I ran challenge/run [cep]* , this made sure that the pattern is matched after the intial letters and covered all 3 files.This gave me the required flag.
```
hacker@globbing~mixing-globs:~$ cd /challenge/files/
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{8DP7rwva5KhP0IX9Zc7d_lTx891.QX1IDO0wiM0EzNzEzW}
```

## What I learned

I learned how to use logic to combine multiple glob patterns to cover all the files I needed. This way i could match many files at once.

## References

none