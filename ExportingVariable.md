# Shell Variable

## Exporting variable
In this challenge, you must invoke /challenge/run with the PWN variable exported and set to the value COLLEGE, and the COLLEGE variable set to the value PWN but not exported (e.g., not inherited by /challenge/run)

### Solve
**Flag:** `pwn.college{wbJYJvzGZHamSCSLZAb9C3pvWHz.QXyYTN0wiN5EzNzEzW}`


```bash
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great 
job! Here is your flag:
pwn.college{wbJYJvzGZHamSCSLZAb9C3pvWHz.QXyYTN0wiN5EzNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$
```

### New Learnings
firstly as in the q it is mentioned that the variable PWN is exported and its value is COLLEGE we run the command
export PWN=COLLEGE
then as per the next line
COLLEGE=PWN (but not exported)
then at last we /challenge/run
