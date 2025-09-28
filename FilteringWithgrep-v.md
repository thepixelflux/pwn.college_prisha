# Practicing Piping

## Filtering with grep -v
In this challenge, /challenge/run will output the flag to stdout, but it will also output over 1000 decoy flags (containing the word DECOY somewhere in the flag) mixed in with the real flag. You'll need to filter out the decoys while keeping the real flag!

Use grep -v to filter out all the lines containing "DECOY" and reveal the real flag!

### Solve
**Flag:** `pwn.college{AUEnJ1sjZMVQwwDYQfsfcwrenoJ.0FOxEzNxwiN5EzNzEzW}`

```bash
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{AUEnJ1sjZMVQwwDYQfsfcwrenoJ.0FOxEzNxwiN5EzNzEzW}
hacker@piping~filtering-with-grep-v:~$ 
```

### New Learnings
writing /challenge/run then pipeline then using grep -v to find the word that is not matching in this case "DECOY"
 
