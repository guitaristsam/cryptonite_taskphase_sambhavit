# Resuming Processes

I learned about the `fg` command which resumes processes that are suspended.
In this question I first ran `/challenge/run` then used `Ctrl+Z` to suspend it, then used the `fg` command to resume it again giving me the flag `pwn.college{ggnjMmM-vnAMEJJPNAunHSC4f3x.dZDN4QDL4gjN0czW}`

```bash
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{ggnjMmM-vnAMEJJPNAunHSC4f3x.dZDN4QDL4gjN0czW}
Don't forget to press Enter to quit me!

Goodbye!
```
