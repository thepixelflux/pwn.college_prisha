# Chaining commands

## Redirecting script output
In this level, we will practice piping (|) from your script to another program. Like before, you need to create a script that calls the /challenge/pwn command followed by the /challenge/college command, and pipe the output of the script into a single invocation of the /challenge/solve command!

### Solve
**Flag:** `pwn.college{0Zkvqf3J6oHfWKmVUW2kZ2VxN60.QX4ETO0wiN5EzNzEzW}`

```bash
hacker@chaining~redirecting-script-output:~$ touch script.sh
hacker@chaining~redirecting-script-output:~$ nano script.sh
hacker@chaining~redirecting-script-output:~$ bash script.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{0Zkvqf3J6oHfWKmVUW2kZ2VxN60.QX4ETO0wiN5EzNzEzW}
hacker@chaining~redirecting-script-output:~$ 
```
### New Learnings
touch -> nano ->enter GNU nano ..inside it ..write ; command to connect two directories..use ctrl x to exit and save...press Y...then press enter
this is how u get out of GNU bash 