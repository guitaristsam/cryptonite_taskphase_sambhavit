# The SUID Bit

Here I learnt about the SUID Bit which makes it so that a file will be executed with the privileges of its owner, instead of the user who runs it.
In this question first I checked the permissions of `/challenge/getroot` using `ls -l`. Then I used `chmod u+s /challenge/getroot` to add the SUID Bit such that whenever it will be executed it will be with the privileges of the owner.
Using this I ran `ls -l /challenge/getroot` to confirm the change, and then ran `/challenge/getroot` which gave me my shell, using which I ran `cat /flag` which gave me the flag `pwn.college{MHqTslITi_T7PbMPvlW6Kiv8gVr.dNTM2QDL4gjN0czW}`

```bash
hacker@permissions~the-suid-bit:~$ ls -l /challenge/getroot
-rwxr-xr-x 1 root root 155 Jul 12 10:30 /challenge/getroot
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ ls -l /challenge/getroot
-rwsr-xr-x 1 root root 155 Jul 12 10:30 /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{MHqTslITi_T7PbMPvlW6Kiv8gVr.dNTM2QDL4gjN0czW}
```
