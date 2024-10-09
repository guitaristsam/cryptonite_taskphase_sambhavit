# Split-piping stderr and stdout

First I executed `/challenge/hack` and this produced both an output and an error. Then I used `> >` to put the output into `/challenge/planet` and `2> >` to put the errors into `/challenge/the`,
thereby satisfying the questions conditions and giving the flag `pwn.college{8O-3QwUk8o6XFo_wbkOY3YHn0-0.dFDNwYDL4gjN0czW}`

```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >( /challenge/planet ) 2> >( /challenge/the )
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{8O-3QwUk8o6XFo_wbkOY3YHn0-0.dFDNwYDL4gjN0czW}
```
