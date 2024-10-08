# Matching with *

First I used `cd` command with `/c*`. Here I used the glob `*` after `c` which makes it so it matches any directory name that starts with `c`. This was to satisfy the condition of using atmost four characters. The shell `/*c` expanded to `/challenge` which combined with the cd command like `cd /challenge` to switch the directory to `/challenge`.
Then I ran `/challenge/run` to get the flag `pwn.college{Yyjz6ahOmABZJlar3Y7V2ONVpcD.dFjM4QDL4gjN0czW}`
```bash
hacker@globbing~matching-with-:~$ cd /c*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{Yyjz6ahOmABZJlar3Y7V2ONVpcD.dFjM4QDL4gjN0czW}
```
