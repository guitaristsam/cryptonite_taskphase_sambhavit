# Matching with [ ]

First I changed the directory to `/challenge/files` using the `cd` command. Then ran `/challenge/run` with the `file_[bash]` argument, giving me the flag `pwn.college{oW4VPM7R2XS8XChRk7UFwz3eT2Z.dNjM4QDL4gjN0czW}`.
This works because `flag_[bash]` becomes `file_b`,`file_a`, `file_s`, `file_h`

```bash
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{oW4VPM7R2XS8XChRk7UFwz3eT2Z.dNjM4QDL4gjN0czW}
```
