# Learning from documentation

Using an example of `ls -a` I understood that `ls` is a command while `-a` is an argument and although `ls` can work by itself it won't show the hidden files as it doesn't show hidden files by default, so it need the `-a` argument like `ls -a` to make sure it also shows the hidden files.
So in this question I ran `/challenge/challenge` with the argument `--giveflag` so that the final command with the argument becomes `/challenge/challenge --giveflag` and gave me the flag `pwn.college{Ic8f_6AUi9ggyByqaLGnJ6O1K9c.dRjM5QDL4gjN0czW}`
```bash
hacker@man~learning-from-documentation:~$ /challenge/challenge --giveflag
Correct argument! Here is your flag:
pwn.college{Ic8f_6AUi9ggyByqaLGnJ6O1K9c.dRjM5QDL4gjN0czW}
```
