# Comprehending Commands

## grepping for a needle a haystack
put a hundred thousand lines of text into the /challenge/data.txt file. grep it for the flag!

### Solve
**Flag:** `pwn.college{wEc6ESVjBNZ-2LoBoFaqkLyRqk3.QX3EDO0wiN5EzNzEzW}`

```bash
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep 'pwn.college' /challenge/data.txt
pwn.college{wEc6ESVjBNZ-2LoBoFaqkLyRqk3.QX3EDO0wiN5EzNzEzW}
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ 
```

### New Learnings
grep [OPTIONS] PATTERN FILE
In this challenge, PATTERN = "pwn.college", FILE = /challenge/data.txt
basg: grep "pwn.college" /challenge/data.txt

Unlike cat (which just prints whole files), grep lets you: Quickly find specific lines inside huge files AND Search across multiple files at once.



