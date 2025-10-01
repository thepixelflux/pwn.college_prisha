# Untangling Users

## Cracking password
Here, John the Ripper cracked Zardus' leaked password hash to find the real value of password1337. Poor Zardus!

This level simulates this story, giving you a leak of /etc/shadow (in /challenge/shadow-leak). Crack it (this could take a few minutes), su to zardus, and run /challenge/run to get the flag!

### Solve
**Flag:** `pwn.college{0jcYBFQEf4nhq5SITNfe0Y1s6I-.QX3UDN1wiN5EzNzEzW}`

```bash
 hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:22 100% 2/3 0.04480g/s 260.8p/s 260.8c/s 260.8C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{0jcYBFQEf4nhq5SITNfe0Y1s6I-.QX3UDN1wiN5EzNzEzW}
zardus@users~cracking-passwords:/home/hacker$
```
### New Learnings
using su command to switch the user then typing the pwd generated
then running /challenge/run again to extract the flag