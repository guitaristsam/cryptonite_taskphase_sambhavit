# Setting PATH

First I overwrote the `PATH` to `/challenge/more_commands`. So that I could run `/challenge/run` invoking win without specifying the full path. Giving me the flag `pwn.college{Ue9yDDETeenU65y0l6GOg6y_g4a.dVzNyUDL4gjN0czW}`

```bash
hacker@path~setting-path:~$ PATH=/challenge/more_commands
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{Ue9yDDETeenU65y0l6GOg6y_g4a.dVzNyUDL4gjN0czW}
```
