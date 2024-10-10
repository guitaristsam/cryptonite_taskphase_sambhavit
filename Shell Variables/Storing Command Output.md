# Storing Command Output

Here I learned about how to store command outputs using `variable=$(command)`. Using this I did `PWN=$(/challenge/run)` which gave me the flag `pwn.college{wRHq75KoppMOC6AzWDRnOWuLE7a.dVzN0UDL4gjN0czW}`

```bash
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{wRHq75KoppMOC6AzWDRnOWuLE7a.dVzN0UDL4gjN0czW}
```
