# Position yet elsewhere

Here, yet again, I did the same thing of running `/challenge/run` to find the correct directory it was located in. Then used change directory `cd` to go to that directory and then ran `/challenge/run` to find the flag `pwn.college{kLjmpeSgJTRx6OcK4BelBwjUaU4.dhDN1QDL4gjN0czW}`

```bash
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /proc/68 directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /proc/68
hacker@paths~position-yet-elsewhere:/proc/68$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{kLjmpeSgJTRx6OcK4BelBwjUaU4.dhDN1QDL4gjN0czW}
```
