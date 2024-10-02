# Implicit relative paths, from /

Here I made the directory to '/' and then ran challenge/run to find the flag

```bash
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{MqvwUm_e03zE4xoQTba7Z72X-Mp.dlDN1QDL4gjN0czW}
```
