# Data Manipulation

## Deleting newlines
use that to read /challenge/read_me into the PWN environment variable, and we'll give you the flag! The /challenge/read_me will keep changing, so you'll need to read it right into the PWN variable with one command!

### Solve
**Flag:** `pwn.college{Ehv29O8iQSawC7QEi9We491zIyk.0VNxEzNxwiN5EzNzEzW}`


```bash
hacker@data~deleting-newlines:~$ /challenge/run | tr -d '\n'
Your line-split flag: pwn.college{Ehv29O8iQSawC7QEi9We491zIyk.0VNxEzNxwiN5EzNzEzW}hacker@data~deleting-newlines:~$  
```
### New Learnings
the general syntax for deleting newlines is 
directoryname | tr -d '\n'
