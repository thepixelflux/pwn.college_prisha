# Comprehending Commands

## ScriptingWithMultipleConditions
For this challenge, write a script at /home/hacker/solve.sh that:

Takes one argument
If the argument is "hack", output "the planet"
If the argument is "pwn", output "college"
If the argument is "learn", output "linux"
For any other input, output "unknown"

### Solve
**Flag:** `pwn.college{IjdBuf1BceXSnwQzczKJsKUClcH.0FOzMDOxwiN5EzNzEzW}`

```bash
hacker@chaining~scripting-with-multiple-conditions:~$ nano solve.sh
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{IjdBuf1BceXSnwQzczKJsKUClcH.0FOzMDOxwiN5EzNzEzW}
hacker@chaining~scripting-with-multiple-conditions:~$
```
### New Learnings
learned softlinks link the file not -the-flag to read out the flag