# Terminal Multiplexing

## Detaching and Attaching
Launch screen
Detach from it.
Run /challenge/run (this will secretly send the flag to your detached session!)
Reattach to see your prize

### Solve
**Flag:** `pwn.college{oxde0IF0P2BVhb5DFfSgkNn6y9G.0lN4IDOxwiN5EzNzEzW}`

```bash
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen
[detached from 147.pts-0.terminal-multiplexing~detaching-and-attaching]
hacker@terminal-multiplexing~detaching-and-attaching:~$ /challenge/run
Found detached screen session: 147.pts-0.terminal-multiplexing~detaching-and-attaching
Sending flag to your screen session...

Flag sent! Now reattach to your screen session with:

  screen -r

You'll find the flag waiting for you there!
```
### New Learnings
Ctrl-A is screen's activation key for all of its shortcuts in its default configuration. All screen functionality is activated by some command combination starting with Ctrl-A.
Hold Ctrl and press A, then release both and press d.
after writing all that code in terminal we write screen -r to get the flag

