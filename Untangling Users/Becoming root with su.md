# Becoming root with su

Here I learnt about `su` which is basically switch user and it allows the user to elevate privileges to root.
First I ran `su` and use the given password `hack-the-planet`, then I used `cat /flag` to get the flag `pwn.college{kicMNB45NCTAgrYND4XI2mz0dwH.dVTN0UDL4gjN0czW}`

```bash
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat /flag
pwn.college{kicMNB45NCTAgrYND4XI2mz0dwH.dVTN0UDL4gjN0czW}
```
