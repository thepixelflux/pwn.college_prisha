# Data Manipulation

## Sorting data
In this challenge, there's a file at /challenge/flags.txt containing 100 fake flags, with the real flag mixed among them. When sorted alphabetically, the real flag will be at the end (we made sure of this when generating fake flags).

### Solve
**Flag:** `pwn.college{ERNO2eqJVLdr8x75u7s8zyEaK_o.0FM0MDOxwiN5EzNzEzW}`


```bash
hacker@data~sorting-data:~$ sort /challenge/flags.txt | tail -n 1
pwn.college{ERNO2eqJVLdr8x75u7s8zyEaK_o.0FM0MDOxwiN5EzNzEzW}
hacker@data~sorting-data:~$   
```
### New Learnings
the file is sorted alphabetically and the real flag is last — -r | head -n 1 reverses so the real flag becomes first, while the second command sorts normally and tail -n 1 picks the last line.