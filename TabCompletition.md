# Files globbing

## Tab Completition
This challenge has copied the flag into /challenge/pwncollege, and you can freely cat that file. But you can't type the filename: we used some serious trickery to make sure that you must tab-complete it. Try it out!

### Solve
**Flag:** `pwn.college{oAgboDoSH2-GqsBgIocEdp8M6_t.0FN0EzNxwiN5EzNzEzW}`

```bash
hacker@globbing~tab-completion:~$ cat /challenge/pwncollege​ 
pwn.college{oAgboDoSH2-GqsBgIocEdp8M6_t.0FN0EzNxwiN5EzNzEzW}
hacker@globbing~tab-completion:~$ 
```

### New Learnings
after reading the content of the /challenge/pwn using cat we press tab then enter.As tempting as it might be, using * to shorten what must be typed on the commandline can lead to mistakes. Your glob might expand to unintended files, and you might not spot it until the rm command is already running! No one is safe from this style of error.A safer alternative when you are trying to specify a specific target is tab completion