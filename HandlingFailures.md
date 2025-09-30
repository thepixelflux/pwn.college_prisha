# Chaining commands

## Chaining iwth semicolons
In this challenge, you need to chain /challenge/first-failure and /challenge/second using the || operator. 

### Solve
**Flag:** `pwn.college{A4i1QR85CLkSB1AqNz6YdXfbYw-.01M0MDOxwiN5EzNzEzW}`

```bash
hacker@chaining~handling-failure:~$ /challenge/first-failure || /challenge/second
Nice chaining! Flag: pwn.college{A4i1QR85CLkSB1AqNz6YdXfbYw-.01M0MDOxwiN5EzNzEzW}
hacker@chaining~handling-failure:~$ 
```
### New Learnings
the || operator allows you to run a second command only if the first command fails (exits with a non-zero code). This is called the "OR" operator because either the first command succeeds OR the second command will run.

command1 || command2
This means: "Run command1, and IF it fails, then run command2.
