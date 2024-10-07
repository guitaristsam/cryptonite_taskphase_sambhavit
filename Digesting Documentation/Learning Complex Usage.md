# Learning Complex Usage

Just tested `/challenge/challenge --printfile /challenge/DESCRIPTION.md` to print out the description of the level
```bash
whacker@man~learning-complex-usage:~$/challenge/challenge --printfile /challenge/DESCRIPTION.md
Correct argument! Here is the /challenge/DESCRIPTION.md file:
While using most commands is straightforward, the usage of some commands can get quite complex.
For example, the arguments to commands like `sed` and `awk`, which we're definitely not getting into right now, are entire programs in an esoteric programming language!
Somewhere on the spectrum between `cd` and `awk` are commands that take arguments to their arguments...

This sounds crazy, but you've already encountered this with the `find` level in [Basic Commands](../commands).
`find` has a `-name` argument, and the `-name` argument itself takes an argument specifying the name to search for.
Many other commands are analogous.

Here is this level's documentation for `/challenge/challenge`:

> Welcome to the documentation for `/challenge/challenge`! This program allows you to print arbitrary files to the terminal, when given the `--printfile` argument. The argument to the `--printfile` argument is the path of the flag to read. For example, `/challenge/challenge --printfile /challenge/DESCRIPTION.md` will print out the description of the level!
Given that documentation, go get the flag!
```
Then I check the files in the directory using the `ls` command
```bash
hacker@man~learning-complex-usage:~$ ls
Desktop  f  flag  not-the-flag  temp
```
Then I used `/challenge/challenge` with the `--printfile` argument, followed by `flag` as the argument to `--printfile`. Which was `/challenge/challenge --printfile flag` and got the flag `pwn.college{wJTjMnIJ4GCc7pm2lZ0IkFPyjLo.dVjM5QDL4gjN0czW}`
```bash
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile flag
Correct argument! Here is the flag file:
pwn.college{wJTjMnIJ4GCc7pm2lZ0IkFPyjLo.dVjM5QDL4gjN0czW}
```
