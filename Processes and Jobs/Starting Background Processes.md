# Starting Background Processes

Here I learnt that instead of starting a process then suspending it using `Ctrl+Z` and then starting it in the background using `bg` we can direcrely use `&` after the command to start it directly in the background, to get the flag `pwn.college{8STtwHzgBsmpk-op14jf3pKdWs_.dlDN4QDL4gjN0czW}`

```bash
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &
[1] 82



Yay, you started me in the background! Because of that, this text will probably
overlap weirdly with the shell prompt, but you're used to that by now...
hacker@processes~starting-backgrounded-processes:~$
Anyways! Here is your flag!
pwn.college{8STtwHzgBsmpk-op14jf3pKdWs_.dlDN4QDL4gjN0czW}

[1]+  Done                    /challenge/run
```
