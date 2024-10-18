# Changing File Ownership

Here I learnt about the `chown` command which is used to change the ownership of files.
Here I change the ownership of the `/flag` file to `hacker` from `root` using `chown`.
Then I used `ls-l` to check ownership of the `/flag` and because it was changer to `hacker` I used the `cat` command to read it and give the flag `pwn.college{IGBbzsISUVdBkJqAAnPkYmaf2i_.dFTM2QDL4gjN0czW}`

```bash
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ ls -l
total 32
-rw-r--r-- 1 hacker hacker    4 Oct  9 13:12 COLLEGE
drwxr-xr-x 2 hacker hacker 4096 Oct  2 05:14 Desktop
-rw-r--r-- 1 hacker hacker    8 Oct  9 14:03 PWN
-rw-r--r-- 1 root   hacker   58 Oct  3 18:42 f
lrwxrwxrwx 1 hacker hacker    5 Oct  7 18:41 flag -> /flag
-rw-r--r-- 1 hacker hacker  829 Oct  9 13:58 instructions
-rw-r--r-- 1 hacker hacker   93 Oct  9 13:58 myflag
lrwxrwxrwx 1 hacker hacker    5 Oct  7 18:43 not-the-flag -> /flag
-rw-r--r-- 1 root   hacker   77 Oct  9 15:07 output
-rw-r--r-- 1 hacker hacker    0 Oct  4 20:40 temp
-rw-r--r-- 1 hacker hacker  435 Oct  9 13:40 the-flag
hacker@permissions~changing-file-ownership:~$ cat flag
pwn.college{IGBbzsISUVdBkJqAAnPkYmaf2i_.dFTM2QDL4gjN0czW}
```
