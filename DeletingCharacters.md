# Data Manipulation

## Deleting Characters
I'll intersperse some decoy characters (specifically: ^ and %) among the flag characters. Use tr -d to remove them!

### Solve
**Flag:** `pwn.college{sQlUSoPzZHLZl7jE0FsH4kWbXFO.0FNxEzNxwiN5EzNzEzW}`


```bash
hacker@data~deleting-characters:~$ /challenge/run | tr -d %^
Your character-stuffed flag:
pwn.college{sQlUSoPzZHLZl7jE0FsH4kWbXFO.0FNxEzNxwiN5EzNzEzW}
hacker@data~deleting-characters:~$ 
```
### New Learnings
the standard syntax for deleting any character  using tr command is:
directoryname | tr -d charyouwannadelete
