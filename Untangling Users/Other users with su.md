# Other users with su

Here I ran the `su` command with the argument `zardus` in order to switch to that user. Then I entered the password `dont-hack-me`, which gave me access to the user.
Then I just ran `/challenge/run` to get the flag `pwn.college{UQGDHgGQQR9gzBMgXBJck333e17.dZTN0UDL4gjN0czW}`

```bash
hacker@users~other-users-with-su:~$ su zardus
Password:
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{UQGDHgGQQR9gzBMgXBJck333e17.dZTN0UDL4gjN0czW}
```
