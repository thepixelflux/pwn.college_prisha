# Terminal Multiplexing

## switching windows
For this challenge, we've set up a screen session with two windows:

Window 0 has... well, you'll have to switch there to find out!
Window 1 has a welcome message

### Solve
**Flag:** `pwn.college{UqVJEGfTEQDhYHGT5GW2boX_-Zf.0FO4IDOxwiN5EzNzEzW}`

```bash
hacker@terminal-multiplexing~switching-windows:~$ screen -r
[detached from 135.challenge_session]
hacker@terminal-multiplexing~switching-windows:~$ 
```
### New Learnings
Ctrl-A c - Create a new window
Ctrl-A n - Next window
Ctrl-A p - Previous window
Ctrl-A 0 through Ctrl-A 9 - Jump directly to window 0-9
Ctrl-A " - bring up a selection menu of all of the windows

all these commands are run in screen -r

