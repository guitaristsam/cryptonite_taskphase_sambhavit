# Position elsewhere

Here, I tried the /challenge/run to get to know which directory I need to be in. Then I went to the /usr/share/build-essential directory and ran /challenge/run to get the flag

```bash
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/build-essential directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /usr/share/build-essential
hacker@paths~position-elsewhere:/usr/share/build-essential$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{cZsj6-9tbdiB-gdL0u98-YI0AL_.ddDN1QDL4gjN0czW}
```
