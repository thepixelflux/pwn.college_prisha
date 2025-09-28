# Practicing Piping

## ProcessSubstitutionForInput
Now for your challenge! Recall what you learned in the diff challenge from Comprehending Commands. In that challenge, you diffed two files. Now, you'll diff two sets of command outputs: /challenge/print_decoys, which will print a bunch of decoy flags, and /challenge/print_decoys_and_flag which will print those same decoys plus the real flag.
Use process substitution with diff to compare the outputs of these two programs and find your flag!

### Solve
**Flag:** `pwn.college{caeUMLj-oMu3Nx5KjNBevp3SQJJ.0lNwMDOxwiN5EzNzEzW}`

```bash
hacker@piping~process-substitution-for-input:~$ diff (/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
bash: syntax error near unexpected token `/challenge/print_decoys'
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
59a60
> pwn.college{caeUMLj-oMu3Nx5KjNBevp3SQJJ.0lNwMDOxwiN5EzNzEzW}
hacker@piping~process-substitution-for-input:~$ 
```

### New Learnings
using diff for comparison and < for process substitution between given 2 files
 
