# Killing Processes

In this module I learnt about how to use the `ps` command in combination with `grep` to locate a process by its command name then I used the `kill` command to terminate it.
First I combined `ps -ef` with `grep` to filter out the `/challenge/dont_run`, I noticed that it was number 73 `(PID)`. Using `kill 73` I succeessfully terminated `/challenge/dont_run`.
Then I just ran `/challenge/run` which gave me the flag `pwn.college{oMrcxz_3JkJFzKEjWjfeY2Fn9bK.dJDN4QDL4gjN0czW}`

```bash
hacker@processes~killing-processes:~$ ps -ef | grep /challenge/dont_run
hacker        73      71  0 15:00 ?        00:00:00 /challenge/dont_run
hacker        97      75  0 15:02 pts/0    00:00:00 grep --color=auto /challenge/dont_run
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{oMrcxz_3JkJFzKEjWjfeY2Fn9bK.dJDN4QDL4gjN0czW}
```
