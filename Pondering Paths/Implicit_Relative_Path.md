# Implicit Relative Path
In this challenge we we run the challenge from /challenge 

## My Solve
**Flag:** 'pwn.college{YCf9PEblGC63H4Av8DKynKWKw5g.QXxUTN0wiM0EzNzEzW}'

First we change our directory to /challenge . we have to run th run command now. the naked command 'run' is genereally not prefered as there could be a prgram of the same name as core system utilities. thus we tell Linux that you explicitly want to execute a program in the current directory, using '.' 

'''
hacker@paths~implicit-relative-path:~$ cd /
hacker@paths~implicit-relative-path:/$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ run
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{YCf9PEblGC63H4Av8DKynKWKw5g.QXxUTN0wiM0EzNzEzW}
hacker@paths~implicit-relative-path:/challenge$
'''


## What I Learned
I learnt how to use cd and go to a specific directory other then '/'. and why we shoudnt use naked commands and specify explicitly the command.  

## References
None.