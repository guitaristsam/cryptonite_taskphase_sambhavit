# Groups and Files

I learnt about the `chgrp` command which is used to change the group who can access to a file, so we can use it to give access to a user part of that group, in this case `hacker`.
First I used `chgrp` to give permission of the file `flag` to the group `hacker`.
Once I had the permission I used the `cat` command to read out the contents of the file `flag` giving me the flag `pwn.college{4HIGdkCutU0zGdgzJOYkgUfe_Nm.dFzNyUDL4gjN0czW}`

```bash
hacker@permissions~groups-and-files:~$ chgrp hacker flag
hacker@permissions~groups-and-files:~$ cat flag
pwn.college{4HIGdkCutU0zGdgzJOYkgUfe_Nm.dFzNyUDL4gjN0czW}
```
