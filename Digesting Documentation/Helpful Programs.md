# Helpful Programs

First I used `/challenge/challenge` with the `--help` argument making it `/challenge/challenge --help`. This gave the optional arguments that I could use with `/challenge/challenge`.
I noticed that there was an argument `-g` for getting the flag but it required a value, so I saw that `-p` would print the value that would cause `-g` to give me the flag
So I ran `/challenge/challenge` with `-p` argument to get the value `274` which helped me run `/challenge/challenge -g 274` and have me the flag `pwn.college{AxIauq2jaYjK7CWTu440sxF358H.ddjM4QDL4gjN0czW}`

```bash
/challenhacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 274
hacker@man~helpful-programs:~$ /challenge/challenge -g 274
Correct usage! Your flag: pwn.college{AxIauq2jaYjK7CWTu440sxF358H.ddjM4QDL4gjN0czW}
```
