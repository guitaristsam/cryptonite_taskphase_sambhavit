# Changing Permissions

I learnt about th `chmod` command which helps to change the permission bits for a file.
Using this I first checked the permissions for the file `/flag` using `ls -l /flag` which told me that only the owner had read permissions for the file. However since I was part of the group `hackers` which had no permissions so couldn't read,write,execute the `/flag` file.
Hence I used the `chmod` command along with `a+rwx flag` which gave everyone (the owner, the group and others not part of both) the permissions to do anything to the file. Then because my user was part of the group even I had the permissions so I did `cat /flag` to get the flag `pwn.college{Imb7a01ERxuIsQQ3LauKEpbq2oZ.dNzNyUDL4gjN0czW}`

```bash
hacker@permissions~changing-permissions:~$ ls -l /flag
-r-------- 1 root root 58 Oct 19 00:27 /flag
hacker@permissions~changing-permissions:~$ chmod a+rwx /flag
hacker@permissions~changing-permissions:~$ ls -l /flag
-rwxrwxrwx 1 root root 58 Oct 19 00:27 /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{Imb7a01ERxuIsQQ3LauKEpbq2oZ.dNzNyUDL4gjN0czW}
```
