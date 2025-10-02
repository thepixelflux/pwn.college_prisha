# Practicing Piping

## Duplicating piped data with tee
This process' /challenge/pwn must be piped into /challenge/college, but you'll need to intercept the data to see what pwn needs from you!

### Solve
**Flag:** `pwn.college{orPpC08PvzbHRzf_nbvIV-XBAG-.QX2EDO0wiN5EzNzEzW}`

```bash
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k challenge]
challenge]: nothing appropriate.
hacker@man~searching-for-manuals:~$ man -k challenge
orpvzbzfnb (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man orpvzbzfnb
hacker@man~searching-for-manuals:~$ /challenge/challenge  --orpvzb 082
Correct usage! Your flag: pwn.college{orPpC08PvzbHRzf_nbvIV-XBAG-.QX2EDO0wiN5EzNzEzW}
hacker@man~searching-for-manuals:~$
```
### New Learnings
-k is command used for searching manual pages listed by man
then finding the argument that contained the command and printing it to get the flag