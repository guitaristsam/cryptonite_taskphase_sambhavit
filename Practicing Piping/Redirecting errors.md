# Redirecting errors

Here I redirected the output and errors of `/challenge/run` using `>` for output and `2>` for errors.
Hence when I ran `/challenge/run > myflag 2> instructions` it redirected my output to the `myflag` file and the errors to the `instruction` file.
Then I used the `cat` command to read the `myflag` file giving me the flag `pwn.college{weXZ-Wk3FdDi9pezBzrcONWN-2R.ddjN1QDL4gjN0czW}`

```bash
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{weXZ-Wk3FdDi9pezBzrcONWN-2R.ddjN1QDL4gjN0czW}

hacker@piping~redirecting-errors:~$ cat instructions
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will check that error output is redirected to a specific file path : instructions
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!

[TEST] You should have redirected my stderr to instructions. Checking...

[PASS] The file at the other end of my stderr looks okay!
[PASS] Success! You have satisfied all execution requirements.
```
