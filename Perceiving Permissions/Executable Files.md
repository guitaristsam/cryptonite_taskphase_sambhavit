# Executable Files

Here I learnt about the execute permissions which is `x`. Here first I used `ls -l /challenge/run` to check the permissons along with the owner and group(which was hacker lol).
Then because my user owned the file but only had permissions to read the file, I used `chmod u+x /challenge/run` , where `u+x` added execute permissions to the hacker user which was because it was the owner of the file.
Then once I had the execute permissions, I simply ran(or executed) `/challenge/run` to get the flag `pwn.college{wU0z9O87P1hEam-72B-ReIvx_Oh.dJTM2QDL4gjN0czW}`

```bash
hacker@permissions~executable-files:~$ ls -l /challenge/run
-r--r--r-- 1 hacker hacker 32 Jul  4 06:37 /challenge/run
hacker@permissions~executable-files:~$ chmod u+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{wU0z9O87P1hEam-72B-ReIvx_Oh.dJTM2QDL4gjN0czW}
```
