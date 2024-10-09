# Mixing globs

First I used the `cd` command to change my current directory to `/challenge/files`. Then I used the `ls` command to list the files in that directory to get an overview of the files I have to work with.
Among these files, I focus on `challenging`, `educational`, and `pwning` which are the files I want to target using the globbing techniques.
Then I executed the command `/challenge/run` with the glob pattern `[cpe]*`.The pattern is designed to match any file that starts with `c`, `p`, or `e`, which are the initial letters of the files I need.
Using this I ran `/challenge/run [cpe]*` which gave me the flag `pwn.college{stUUtE3sAIxU1i0Y3tMmBU5la5K.dVjM4QDL4gjN0czW}`

```bash
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ ls
amazing      delightful   great       jovial    magical     pwning   splendid   victorious  youthful
beautiful    educational  happy       kind      nice        queenly  thrilling  wonderful   zesty
challenging  fantastic    incredible  laughing  optimistic  radiant  uplifting  xenial
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cpe]*
You got it! Here is your flag!
pwn.college{stUUtE3sAIxU1i0Y3tMmBU5la5K.dVjM4QDL4gjN0czW}
```
