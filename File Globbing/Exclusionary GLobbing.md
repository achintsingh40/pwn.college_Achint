# Exclusionary GLobbing

We are supposed to run all the files that don't start with a p,w or n.

**Flag:** `pwn.college{o0y78j4DBYcRPxmlvokw6sfrXQn.QX2IDO0wiM0EzNzEzW}`


```
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files/
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{o0y78j4DBYcRPxmlvokw6sfrXQn.QX2IDO0wiM0EzNzEzW}
```

## What I learned

We learned about exclusionary globbing, which works the opposite way from globbing . Normally, globbing helps us find files that contain certain letters or patterns. But with exclusionary globbing, we use ! or ^ inside square brackets [] to match files that do not include certain characters. This special way of excluding characters only works inside the square brackets part of the pattern.
## References

noen