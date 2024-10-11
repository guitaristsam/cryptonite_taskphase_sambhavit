# Suspending Processes

Here I learnt about `Ctrl+Z` which can suspend processes to the background. Here I first ran `/challenge/run` and suspended it with `Ctrl+Z` then I ran another `/challenge/run` while the first one was suspended which gave me the flag `pwn.college{8RLnWig9-fzeBjsYJyGb6nstvS3.dVDN4QDL4gjN0czW}`

```bash
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          85      65  0 16:48 pts/0    00:00:00 bash /challenge/run
root          87      85  0 16:48 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          85      65  0 16:48 pts/0    00:00:00 bash /challenge/run
root          92      65  0 16:48 pts/0    00:00:00 bash /challenge/run
root          94      92  0 16:48 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{8RLnWig9-fzeBjsYJyGb6nstvS3.dVDN4QDL4gjN0czW}
```
