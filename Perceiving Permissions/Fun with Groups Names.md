# Fun with Groups Names

Here the question specified that the user was not in the default group `hacker`. So I used `id` to check which group my user was in, Once I found out I was in `grp13758` I used the `chgrp` command to change the group to `grp13758` for the file flag.
Then once I had the permission I used the `cat` command to read out the contents of the `flag` file giving me the flag `pwn.college{oX734dAdPiVFIS8XQHxNb3z0tsW.dJzNyUDL4gjN0czW}`

```bash
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp13758) groups=1000(grp13758)
hacker@permissions~fun-with-groups-names:~$ chgrp grp13758 flag
hacker@permissions~fun-with-groups-names:~$ cat flag
pwn.college{oX734dAdPiVFIS8XQHxNb3z0tsW.dJzNyUDL4gjN0czW}
```
