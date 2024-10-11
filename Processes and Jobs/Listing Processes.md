# Listing Processes

In this module I learnt about similarities and differences between `ps -ef` and `ps aux` commands.
Using this knowledge I used `ps -ef` command first because I knew that my challenge file was already running, and I needed to locate it.
I noticed the command` /challenge/28190-run-32370` and running this gave me the flag `pwn.college{cqo-JxIfCkUGjql4v3_rbrO8o55.dhzM4QDL4gjN0czW}`

```bash
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 11:39 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bin/dojo-init /ru
root           7       1  0 11:39 ?        00:00:00 /run/dojo/bin/sleep 6h
root          68       1  0 11:39 ?        00:00:00 /challenge/28190-run-32370
root          72      68  0 11:39 ?        00:00:00 sleep 6h
hacker        73       0  0 11:40 pts/0    00:00:00 /run/dojo/bin/ssh-entrypoint
hacker        90      73  0 11:40 pts/0    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/28190-run-32370
Yahaha, you found me! Here is your flag:
pwn.college{cqo-JxIfCkUGjql4v3_rbrO8o55.dhzM4QDL4gjN0czW}
Now I will sleep for a while (so that you could find me with 'ps').
```
