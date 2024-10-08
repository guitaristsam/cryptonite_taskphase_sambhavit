# Help for Builtins

First I used the `help` command to get information about `challenge` command. This gave me the options I could use as arguments for `challenge`.
I saw that the right value for `--secret` was `kyfkeSQ_` so I ran the `challenge` command with `--secret kyfkeSQ_` as the argument, `challenge --secret kyfkeSQ_` which gave me the flag `pwn.college{kyfkeSQ_YI2XDjPBBMSS7EQvKBI.dRTM5QDL4gjN0czW}`

```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "kyfkeSQ_".
hacker@man~help-for-builtins:~$ challenge --secret kyfkeSQ_
Correct! Here is your flag!
pwn.college{kyfkeSQ_YI2XDjPBBMSS7EQvKBI.dRTM5QDL4gjN0czW}
```
