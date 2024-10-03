# home sweet home

This worked because `~/f` is three characters before expansion and becomes an absolute path inside `/home/hacker`, meeting the challenge’s requirements

```bash
hacker@paths~home-sweet-home:~$ /challenge/run ~/f
Writing the file to /home/hacker/f!
... and reading it back to you:
pwn.college{AVs4uMiReAKF653G67-V0ASSPRb.dNzM4QDL4gjN0czW}
```
