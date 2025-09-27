# Grepping for a needle in a haystack

We need to invoke the grep command to find the flag amongst thousand lines of code in a file.


**Flag:** `pwn.college{A-66T83Pgi4KQWXsMxFkHFK2hPs.QX3EDO0wiM0EzNzEzW}`
We are using the grep command to find the flag from thousand line code. the syntax of grep command is 'grep SEARCH_STRING /path/to/file'. Here the given the search_string would be pwn.college as the grep command searches the file for any code containing the particular search string.

```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{A-66T83Pgi4KQWXsMxFkHFK2hPs.QX3EDO0wiM0EzNzEzW}
```

## What I learned

I learnt that the grep command is used to find a specific string from a very long code and how to use it .

## References

none
