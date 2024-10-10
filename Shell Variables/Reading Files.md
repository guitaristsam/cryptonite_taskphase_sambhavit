# Reading Files

In this challenge I learnt how to read files with the shell.
Here when the `read` command reads into the variable `PWN` it reads from `/challenge/read_me` instead.
Which is why running `read PWN < /challenge/read_me` gave me the flag `pwn.college{EoJD8P3TWBdYL93uSfE1IRsI2vi.dBjM4QDL4gjN0czW}`

```bash
hacker@variables~reading-files:~$  read PWN < /challenge/read_me
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{EoJD8P3TWBdYL93uSfE1IRsI2vi.dBjM4QDL4gjN0czW}
```
