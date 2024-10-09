# Writing to mulitple programs

First I ran `/challenge/hack` and simultaneously duplicated its output as input to both `/challenge/the` and `/challenge/planet` using the pipe(`|`) operator to take the output of `/challenge/hack` and the `tee` command to to split the output stream so that it can be sent to both `/challenge/the`, and `/challenge/planet`.
Running `/challenge/hack | tee >(/challenge/planet) >(/challenge/the)` gave me the flag `pwn.college{gRrAElo_24cYvXmXbmr3Pe3zrXi.dBDO0UDL4gjN0czW}`
```bash
hacker@piping~writing-to-multiple-programs:~$  /challenge/hack | tee >(/challenge/planet) >(/challenge/the)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
1451616847253117403
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{gRrAElo_24cYvXmXbmr3Pe3zrXi.dBDO0UDL4gjN0czW}
```
