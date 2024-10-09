# Duplicating piped data with tee

First I executed the `/challenge/pwn` command and piped its output into the `tee` command. The `tee` command allowed me to duplicate the output stream, sending it to a file `output`,
while also passing it to the `/challenge/college` command. This way I could see what `/challenge/pwn` was producing using the `output` file and also provide that output to `/challenge/college`.
Then I got to know that `/challenge/pwn --secret [SECRET_ARG]` will print the flag if `[SECRET_ARG]` was `EFs1bMxX`.
I ran the `/challenge/pwn` command again, this time with the `--secret` option set to `EFs1bMxX`, and piped its output directly into the `/challenge/college` command to get the flag `pwn.college{EFs1bMxX236ckNV_P-pTDD_QNx7.dFjM5QDL4gjN0czW}`



```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee output | /challenge/college
Processing...
WARNING: you are overwriting file output with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat output
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "EFs1bMxX"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret EFs1bMxX | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{EFs1bMxX236ckNV_P-pTDD_QNx7.dFjM5QDL4gjN0czW}
```
