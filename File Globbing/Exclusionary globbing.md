# Exclusionary globbing

First I changed my current directory to `/challenge/files` using the `cd` command. Then I ran `challenge/run` with `[!pwn]*` as the argument so that it doesn't match with any file that does not start with the letters `p`, `w` or `n` by utilizing `!` which makes it so it excludes any files that begin with these characters.
Using this I got the flag `pwn.college{0Es4RONb31iZvPc9ANUOdcVs8CU.dZjM4QDL4gjN0czW}`

```bash
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{0Es4RONb31iZvPc9ANUOdcVs8CU.dZjM4QDL4gjN0czW}
```
