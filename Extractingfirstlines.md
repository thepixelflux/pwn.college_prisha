# Dara Manipulation

## Extracting first lines with head
This challenge's /challenge/pwn outputs a bunch of data, and you'll need to pipe it through head to grab just the first 7 lines and then pipe them onwards to /challenge/college, which will give you the flag if you do this right! Your solution will be a long composite command with two pipes connecting three commands

### Solve
**Flag:** `pwn.college{g_gpNjldewdZtq6vsoAKuPN-Zg1.0lNxEzNxwiN5EzNzEzW}`

```bash
hacker@data~extracting-the-first-lines-with-head:~$ /challenge/pwn | head -n 7 | /challenge/college
Congratulations, you piped the right codes!
pwn.college{g_gpNjldewdZtq6vsoAKuPN-Zg1.0lNxEzNxwiN5EzNzEzW}
hacker@data~extracting-the-first-lines-with-head:~$ 
```
### New Learnings
the syntax for the same is:
directoryname | head -n x | directoryname
x=no of first lines u wanna print
