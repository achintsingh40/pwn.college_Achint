explicit relative apths, from / 
earlier, our relative path was naked, it directly specified the directory to descend into from the current directory.In this challenge we need to run a relative dircetory '/', and then run the challenge command beginning with '.'  

## My Solve
**Flag:** 'pwn.college{4L0pVfogA4SZGYg0Hbt31Y02PIs.QXwUTN0wiM0EzNzEzW}'

First we check which directory are we in then we go to the relative directory '/'. Now we have to run the challenge command, when we try to do it, it tells that this challenge needs to be  called with a relative path that explicitly starts with a '.' . we type the command in the given specific way ./././challenge/run or  ./challenge/run both work.

```
hacker@paths~explicit-relative-paths-from-:/challenge$ cd /
hacker@paths~explicit-relative-paths-from-:/$ pwd
/
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{4L0pVfogA4SZGYg0Hbt31Y02PIs.QXwUTN0wiM0EzNzEzW}

hacker@paths~explicit-relative-paths-from-:/$ pwd
/
hacker@paths~explicit-relative-paths-from-:/$ ./././challenge/run
Correct!!!
./././challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{4L0pVfogA4SZGYg0Hbt31Y02PIs.QXwUTN0wiM0EzNzEzW}
hacker@paths~explicit-relative-paths-from-:/$
```

## What I Learned
I learnt about paths explicitely starting with '.'. they are more relative explicit paths and how they are run.      

## References
None.