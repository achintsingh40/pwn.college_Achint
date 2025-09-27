# An Epic Filesystem Quest

We are given a little game in which we have to solve using hints given by the system using cd, ls and cat. The first clue is to use / as our working directory and find a file named clue or something similar using ls, we are then supposed to use the clues till we get the flag.

**Flag:** `pwn.college{kg1yQCgxBnATofS8-SPOsGKQQQm.QX5IDO0wiM0EzNzEzW}`
 I first used 'cd /' to navigate to / directory as said in the challenge then i followed the clues as they told to do. we used cat, ls, ls -a,cd to read files which were hidden with and wihtout using cd.

```
hacker@commands~an-epic-filesystem-quest:/challenge$ cd /
hacker@commands~an-epic-filesystem-quest:/$ cat SNIPPET
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/babel/localtime/__pycache__

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/python3/dist-packages/babel/localtime/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/babel/localtime/__pycache__$ ls
REVELATION  __init__.cpython-38.pyc  _unix.cpython-38.pyc  _win32.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/babel/localtime/__pycache__$ cat REVELATION
Congratulations, you found the clue!
The next clue is in: /usr/lib/debug/.build-id/9b
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/babel/localtime/__pycache__$ cd /usr/lib/debug/.build-id/9b
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/9b$ ls
217a1939de77ad7110f8eaf640c650ddcbfe51.debug  LEAD
97e3e47d04aeeac8ba47b8c93a4b87a7a5d632.debug  c60746b0fb95ff966ceaf2f7f6f71c6cb1c3ab.debug
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/9b$ cat LEAD
Congratulations, you found the clue!
The next clue is in: /opt/linux/linux-5.4/include/config/logitech

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/9b$ cat /opt/linux/linux-5.4/include/config/logitech
cat: /opt/linux/linux-5.4/include/config/logitech: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/9b$ ls /opt/linux/linux-5.4/include/config/logitech
INFO-TRAPPED  ff.h
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/9b$ cat /opt/linux/linux-5.4/include/config/logitech/INFO-TRAPPED
Great sleuthing!
The next clue is in: /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/SansSerif/Regular

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/debug/.build-id/9b$ cd /usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/SansSerif/Regular
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/SansSerif/Regular$ ls
Main.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/SansSerif/Regular$ ls -a
.  ..  .CUE  Main.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/SansSerif/Regular$ cat .
cat: .: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/SansSerif/Regular$ cd .
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/SansSerif/Regular$ ls
Main.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/SansSerif/Regular$ ls -a
.  ..  .CUE  Main.js
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/SansSerif/Regular$ cat .CUE
Great sleuthing!
The next clue is in: /usr/share/sphinx/locale/tr
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/jax/output/HTML-CSS/fonts/Asana-Math/SansSerif/Regular$ cd /usr/share/sphinx/locale/tr
hacker@commands~an-epic-filesystem-quest:/usr/share/sphinx/locale/tr$ ls
TIP  sphinx.js
hacker@commands~an-epic-filesystem-quest:/usr/share/sphinx/locale/tr$ ls -a
.  ..  TIP  sphinx.js
hacker@commands~an-epic-filesystem-quest:/usr/share/sphinx/locale/tr$ cat TIP
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/include/uapi/linux/sched
hacker@commands~an-epic-filesystem-quest:/usr/share/sphinx/locale/tr$ cd /opt/linux/linux-5.4/include/uapi/linux/sched
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/uapi/linux/sched$ ls
DOSSIER  types.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/uapi/linux/sched$ cat DOSSIER
Lucky listing!
The next clue is in: /opt/busybox/busybox-1.33.2/arch/x86_64

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/uapi/linux/sched$ cd /opt/busybox/busybox-1.33.2/arch/x86_64
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/arch/x86_64$ ls
EVIDENCE  Makefile
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/arch/x86_64$ cat EVIDENCE
Great sleuthing!
The next clue is in: /usr/lib/python3/dist-packages/sphinx/writers/__pycache__

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/arch/x86_64$ ls /usr/lib/python3/dist-packages/sphinx/writers/__
pycache__
NUGGET-TRAPPED           html.cpython-38.pyc   latex.cpython-38.pyc    texinfo.cpython-38.pyc  websupport.cpython-38.pyc
__init__.cpython-38.pyc  html5.cpython-38.pyc  manpage.cpython-38.pyc  text.cpython-38.pyc     xml.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/arch/x86_64$ cat  /usr/lib/python3/dist-packages/sphinx/writers/__pycache__/NUGGET-TRAPPED
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{kg1yQCgxBnATofS8-SPOsGKQQQm.QX5IDO0wiM0EzNzEzW}
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/arch/x86_64$
```

## What I learned

It was a kidn of revision of all commands learnt till now

## References

none
