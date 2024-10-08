# Searching Manuals

Here First I used the `man` command with `challenge` argument to read the manual for `challenge` then I used `/flag` to search for the right argument to use in order to get the flag. Used `N` and `n` to navigate through the results and found out `--gu This argument will give you the flag!` then used `/challenge/challenge --gu` in order to get the flag `pwn.college{IN2ZMRjVI3xZJyrewn9atkzMBYt.dVTM4QDL4gjN0czW}` 

```bash
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --gu
Initializing...
Correct usage! Your flag: pwn.college{IN2ZMRjVI3xZJyrewn9atkzMBYt.dVTM4QDL4gjN0czW}
```
