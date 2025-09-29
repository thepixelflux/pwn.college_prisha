# Untangling Users

## Becoming root with su
But THIS challenge (and only this challenge) does have a root password. That password is hack-the-planet, and you must provide it to su to become root! Go do that, and read the flag!

### Solve
**Flag:** `pwn.college{U_Iea_30sLyev-xK__J5Hn0d18i.QX1UDN1wiN5EzNzEzW}`

```bash
hacker@users~becoming-root-with-su:~$ su
Password: 
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{U_Iea_30sLyev-xK__J5Hn0d18i.QX1UDN1wiN5EzNzEzW}
root@users~becoming-root-with-su:/home/hacker# 
```
### New Learnings
using the su command to access the flag