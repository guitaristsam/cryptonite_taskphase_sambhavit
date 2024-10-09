# Redirecting more output

First I redirected my output of `/challenge/run` to the `myflag` file using the `>` operator. Then used the `cat` command to read the contents of the `myflag` file that gave me the flag `pwn.college{oyujlomkHZopj-gIpVPnKc95Wn6.dVjN1QDL4gjN0czW}`

```bash
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{oyujlomkHZopj-gIpVPnKc95Wn6.dVjN1QDL4gjN0czW}
```
