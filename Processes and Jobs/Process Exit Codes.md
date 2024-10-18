# Process Exit Codes

Here I learnt that I can use `$?` after a command to access its exit code. 
First I used the `echo` command with `$?` to access its exit code and it returned 0.
Then I ran `/challenge/get-code` and it exited with an error code.
Then used `$?` to get an exit code which was `110`.
Then I ran `/challenge/submit-code 110` which gave me the flag `pwn.college{EakAqlO7R0DtX5te3aLpXjGaNmV.dljN4UDL4gjN0czW}`

```bash
hacker@processes~process-exit-codes:~$ echo $?
0
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
110
hacker@processes~process-exit-codes:~$ /challenge/submit-code 110
CORRECT! Here is your flag:
pwn.college{EakAqlO7R0DtX5te3aLpXjGaNmV.dljN4UDL4gjN0czW}
```
