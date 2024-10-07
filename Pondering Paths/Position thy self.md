# Position thy self

Here the initial directory was `~` but `/challenge/run` was not in the `~` directory so used the change directory ,`cd` command to change to `tmp` directory and then executed `/challenge/run` to find flag `pwn.college{kwW2WeLf2VUN74ICFZK-hfmONHM.dZDN1QDL4gjN0czW}`

```bash
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /tmp directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /tmp
hacker@paths~position-thy-self:/tmp$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{kwW2WeLf2VUN74ICFZK-hfmONHM.dZDN1QDL4gjN0czW}
```
