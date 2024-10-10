# Multi-word Variables

Here I learned that if I need to set a variable to a value with a two words then it needs to be in double quotes otherwise it will interpret the second word as a command.
For example if I had done `PWN=COLLEGE YEAH` instead then `YEAH` would have been taken as a command.
So to avoid that I did `PWN="COLLEGE YEAH"` with double quotes instead to get the flag `pwn.college{cUl0LWsoOOaXIfn1eCnEnVoXxve.dBjN1QDL4gjN0czW}`.

```bash
hacker@variables~multi-word-variables:~$ PWN="COLLEGE YEAH"
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{cUl0LWsoOOaXIfn1eCnEnVoXxve.dBjN1QDL4gjN0czW}
```
