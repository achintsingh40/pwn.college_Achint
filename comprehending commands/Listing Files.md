# Listing Files

We are supposed to list the files under /challenge to find what the required program file is called and hence run it to obtain the required flag

**Flag:** `pwn.college{wYoMhzwZtuvFB-Nrav--dPeLwf5.QX4IDO0wiM0EzNzEzW}`
First I lsited all the files under /challenge to see what the run file has been renamed to. IT was renamed to 27460-renamed-run-29171. then after running /challenge/27460-renamed-run-29171 , i got the flag. I coudnt figure out how to get the flag when i used the'cat /challenge/27460-renamed-run-29171'command. #!/opt/pwn.college/bash  

echo "Yahaha, you found me! Here is your flag:"
cat /flag
this had come as a output. 
when i wrote /flag it showed  Permission denied.
then i tried multiple commands and got to the solution.

```
hacker@commands~listing-files:~$ ls /challenge
27460-renamed-run-29171  DESCRIPTION.md
hacker@commands~listing-files:~$ cat /challenge/27460-renamed-run-29171
#!/opt/pwn.college/bash

echo "Yahaha, you found me! Here is your flag:"
cat /flag
hacker@commands~listing-files:~$ echo "Yahaha, you found me! Here is your flag:"
cat /flag
Yahaha, you found me! Here is your flag:
cat: /flag: Permission denied
hacker@commands~listing-files:~$ /challenge/27460-renamed-run-29171
Yahaha, you found me! Here is your flag:
pwn.college{wYoMhzwZtuvFB-Nrav--dPeLwf5.QX4IDO0wiM0EzNzEzW}
```

## What I learned

I learnt how ls is used to list the content of a directory and how it may help us navigate the contents of a directory

## References

none