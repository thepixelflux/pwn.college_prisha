# Practicing Piping

## Redirecting more output
Add challenge description here

### Solve
**Flag:** `pwn.college{QQn-t1kYTgubMOIXPzGUPNqYs7J.QX1YTN0wiN5EzNzEzW}`

type in your solve and your thought process behind solving the challenge. Include as much as info as possible. Use triple ticks for any bash commands and output you type on the terminal.

```bash
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{QQn-t1kYTgubMOIXPzGUPNqYs7J.QX1YTN0wiN5EzNzEzW}
```

### New Learnings
#- /challenge/run → runs the program that gives you the flag. → redirects standard output (stdout) to a file by using > ..myflag → the file where stdout will be written and we can print the contents of it .(your flag will be saved here).
