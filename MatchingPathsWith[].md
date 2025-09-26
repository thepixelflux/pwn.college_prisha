# files globbing

## Matching paths with []
we've placed a bunch of files in /challenge/files. Starting from your home directory, run /challenge/run with a single argument that bracket-globs into the absolute paths to the file_b, file_a, file_s, and file_h files!

### Solve
**Flag:** `pwn.college{8uHQE4HOdj4PGA6dehxAPW6nNs1.QX0IDO0wiN5EzNzEzW}`

```bash
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{8uHQE4HOdj4PGA6dehxAPW6nNs1.QX0IDO0wiN5EzNzEzW}
hacker@globbing~matching-paths-with-:~$ 
```

### New Learnings
/challenge/files
challenge = a directory under the root /.Inside that, there is an entry called files.Since the statement said “we’ve placed a bunch of files in /challenge/files”, that means files is itself a directory.
Inside /challenge/files/, you have file_a, file_b, file_s, file_h, etc.

/challenge/run: This is a file, not a directory.

A file name does not have to be just a single word like abc.A “name” can include / if you’re writing the path to the file.
Example: xyz/yui means:
xyz is a directory.yui is a file inside xyz.
So technically, xyz/yui is not the name of a single file — it’s a path (directory + filename).
