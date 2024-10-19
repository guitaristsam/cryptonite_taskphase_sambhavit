# The PATH Variable

I set `PATH="rm"` in my shell. This overwrote the default `PATH`, so the shell could no longer find the `rm` command when `/challenge/run` tried to execute it.
Which gave me the flag `pwn.college{4FNkkDKYT_nZO6XPXjrBeWQNR-7.dZzNwUDL4gjN0czW}`

```bash
hacker@path~the-path-variable:~$ PATH="rm"
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: command not found
The flag is still there! I might as well give it to you!
pwn.college{4FNkkDKYT_nZO6XPXjrBeWQNR-7.dZzNwUDL4gjN0czW}
```
