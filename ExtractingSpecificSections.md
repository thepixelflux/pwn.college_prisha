# Data Manipulation

## Extracting specific sections
In this challenge, the /challenge/run program will give you a bunch of lines with random numbers and single characters (characters of the flag) as columns. Use cut to extract the flag characters, then pipe them to tr -d "\n" (like the previous level!) to join them together into a single line. Your solution will look something like /challenge/run | cut ??? | tr ???, with the ??? filled out.

### Solve
**Flag:** `pwn.college{ca0NYlEKx__CA1qG7PUJGr8UNJx.01NxEzNxwiN5EzNzEzW}`


```bash
hacker@data~extracting-specific-sections-of-text:~$ /challenge/run | cut -d " " -f 2 | tr -d '\n'
pwn.college{ca0NYlEKx__CA1qG7PUJGr8UNJx.01NxEzNxwiN5EzNzEzW}hacker@data~extracting-specific-sections-of-text:~$  
```
### New Learnings
cut -d " ": use a space as the field delimiter.
-f 2: extract field (column) 2 from each line (change 2 to the correct column if needed).
tr -d '\n': remove newlines so all characters join into a single line (the flag).

If the character is in a different column, change -f 2 to that number (e.g. -f 3).