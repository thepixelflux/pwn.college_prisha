# File globbing

## Multiple options for tab completition
This challenge has a /challenge/files directory with a bunch of files starting with pwncollege. Tab-complete from /challenge/files/p or so, and make your way to the flag!

### Solve
**Flag:** `pwn.college{QtqosWyAOQRgbqf1U7Y8TAUdadX.0lN0EzNxwiN5EzNzEzW}`

```bash
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn
pwn                    pwn-the-planet         pwncollege-flag        pwncollege-flyswatter
pwn-college            pwncollege-family      pwncollege-flamingo    pwncollege-hacking
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-
pwncollege-family      pwncollege-flag        pwncollege-flamingo    pwncollege-flyswatter  pwncollege-hacking
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-fl
pwncollege-flag        pwncollege-flamingo    pwncollege-flyswatter
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-fla
pwncollege-flag      pwncollege-flamingo
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-fla
pwncollege-flag      pwncollege-flamingo
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-flag
pwn.college{QtqosWyAOQRgbqf1U7Y8TAUdadX.0lN0EzNxwiN5EzNzEzW}
hacker@globbing~multiple-options-for-tab-completion:~$
```
### New Learnings
using tab command to get the flag