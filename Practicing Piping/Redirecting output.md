# Redirecting output

First, I used the command `echo` to print `PWN` but redirected that output of it to the file `COLLEGE`. The `>` operator redirects the output from the echo command into the file instead of being displayed in the terminal.
So running `echo PWN > COLLEGE` gave me the flag `pwn.college{Q-a47zewOl3NGrTyIgULFYRxjLI.dRjN1QDL4gjN0czW}`

```bash
hacker@piping~redirecting-output:~$ echo PWN > COLLEGE
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your
flag:
pwn.college{Q-a47zewOl3NGrTyIgULFYRxjLI.dRjN1QDL4gjN0czW}
```
