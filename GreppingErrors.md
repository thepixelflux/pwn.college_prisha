# Practicing Piping

## Grepping Errors
The shell has a >& operator, which redirects a file descriptor to another file descriptor. This means that we can have a two-step process to grep through errors: first, we redirect standard error to standard output (2>& 1) and then pipe the now-combined stderr and stdout as normal (|)!
Try it now! Like the last level, this level will overwhelm you with output, but this time on standard error. grep through it to find the flag!

### Solve
**Flag:** `pwn.college{UNE92RDRQVFp_9jQPd1spxbqD0A.QX1ATO0wiN5EzNzEzW}`

```bash
hacker@piping~grepping-errors:~$ /challenge/run |& grep "pwn.college"
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{UNE92RDRQVFp_9jQPd1spxbqD0A.QX1ATO0wiN5EzNzEzW}
hacker@piping~grepping-errors:~$
```

### New Learnings
|& is equivalent to 2>&1 |
dup file descriptor 2 (stderr) to whatever file descriptor 1 (stdout) currently refers to.
 
