# Practising piping

## Named pipes
This challenge will be a simple introduction to FIFOs. You'll need to create a /tmp/flag_fifo file and redirect the stdout of /challenge/run to it. If you're successful, /challenge/run will write the flag into the FIFO! Go do it!

HINT: The blocking behavior of FIFOs makes it hard to solve this challenge in a single terminal. You may want to use the Desktop or VSCode mode for this challenge so that you can launch two terminals.

### Solve
**Flag:** `pwn.college{kYw5w8rRo1pTvJp6M7_AJpjneJ0.01MzMDOxwiN5EzNzEzW}`

```bash
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
cat: /tmp/flag_fifo: No such file or directory
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at 
/tmp/flag_fifo! Here is your flag:
pwn.college{kYw5w8rRo1pTvJp6M7_AJpjneJ0.01MzMDOxwiN5EzNzEzW}
hacker@piping~named-pipes:~$  
```
### New Learnings
we can also create your own persistent named pipes that stick around on the filesystem! These are called FIFOs, which stands for First (byte) In, First (byte) Out.