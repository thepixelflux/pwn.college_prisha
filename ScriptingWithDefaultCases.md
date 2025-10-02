# Chaining commands

## ScriptingWithDefaultCases
For this challenge, write a script at /home/hacker/solve.sh that:

Takes one argument
If the argument is "pwn", output "college"
For any other input, output "nope"


### Solve
**Flag:** `pwn.college{wUtRnf9nnaGdYycvXylWUyaMG2m.01NzMDOxwiN5EzNzEzW}`

```bash
hacker@chaining~scripting-with-default-cases:~$ nano solve.sh
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{wUtRnf9nnaGdYycvXylWUyaMG2m.01NzMDOxwiN5EzNzEzW}
```
### New Learnings
in the bash we write:
#!/bin/sh

if [ "$1" = "pwn" ]; then
  echo  "college"
else
  echo "nope"
fi
