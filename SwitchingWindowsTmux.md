# Terminal Multiplexing

## Switching windows
We've created a tmux session with two windows:

Window 0 has the flag!
Window 1 has your warm welcome.
Go get that flag!

### Solve
**Flag:** ` pwn.college{ssSzW7mcj4ylgY80_wgwcBYGUpO.0FM5IDOxwiN5EzNzEzW}`

```bash
hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{ssSzW7mcj4ylgY80_wgwcBYGUpO.0FM5IDOxwiN5EzNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{ssSzW7mcj4ylgY80_wgwcBYGUpO.0FM5IDOxwiN5EzNzEzW}
hacker@terminal-multiplexing~switching-windows-tmux:~$
```
### New Learnings
first we do tmux a...we go inside the tmux window .... ctrl b 0 to window 0 which has the flag