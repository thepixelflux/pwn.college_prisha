# Data Manipulation

## Translating Characters
/challenge/run will print the flag but will swap the casing of all characters (e.g., A will become a and vice-versa). Can you undo it with tr and get the flag?

### Solve
**Flag:** `pwn.college{QLTfWDC6H4E_JQQvAqAzaVwkHDT.01MxEzNxwiN5EzNzEzW}`


```bash
hacker@data~translating-characters:~$ /challenge/run | tr 'A-Za-z' 'a-zA-Z'
yOUR CASE-SWAPPED FLAG:
pwn.college{QLTfWDC6H4E_JQQvAqAzaVwkHDT.01MxEzNxwiN5EzNzEzW}

hacker@data~translating-characters:~$ 
```
### New Learnings
putting what u want to assign to a variable in ""
