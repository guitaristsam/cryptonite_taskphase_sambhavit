# Matching with ?

Here I used `cd` command to change directrory but used it with `/?ha??enge`, by replacing `c` and `l` with `?` instead. `?` only matches itself to one character making it `/challenge` so with `cd` it becomes `cd /challenge`.
Then I ran `/challenge/run` to get the flag `pwn.college{ICi-gFig3HZey-RAsC2Qob5AYwr.dJjM4QDL4gjN0czW}`

```bash
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{ICi-gFig3HZey-RAsC2Qob5AYwr.dJjM4QDL4gjN0czW}
```
