# Foregrounding Processes

Here I learnt about the `fg` command which brings a background process to the foreground.
First I ran `/challenge/run` then used `Ctrl+Z` to suspend the process, then used `bg` command to resume `/challenge/run` in the background and then used `fg` command to resume it to the foreground,
giving the flag `pwn.college{EcU8Rf86SSNJSn-V8RpAuvv_6Tm.dhDN4QDL4gjN0czW}`

```bash
hacker@processes~foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the
background, and *then* foreground it without re-suspending it! You can
background me with Ctrl-Z (and resume me in the background with 'bg') or, if
you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ bg
[1]+ /challenge/run &



Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out. After that, resume me into the foreground with 'fg';
I'll wait.
hacker@processes~foregrounding-processes:~$ fg
/challenge/run
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!

pwn.college{EcU8Rf86SSNJSn-V8RpAuvv_6Tm.dhDN4QDL4gjN0czW}
```
