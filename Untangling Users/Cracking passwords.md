# Cracking passwords

First I used `cat /challenge/shadow-leak` to find out the password of zardus. I found the password however it was the result of one-way-encrypting.Hence I used the famous John the Ripper method 
by running `john /challenge/shadow-leak` which gave me the decrypted password. Once I found that the password for the user `zardus` was `aardvark`, I used `su zardus` to switch user to zardus using the obtained password.
Once I was the `zardus` user I ran `/challenge/run` to find the flag `pwn.college{cBSSdtSjQnUALsVBmpyHPWhaX_E.ddTN0UDL4gjN0czW}`

```bash
hacker@users~cracking-passwords:~$ cat /challenge/shadow-leak
root:*:19873:0:99999:7:::
daemon:*:19873:0:99999:7:::
bin:*:19873:0:99999:7:::
sys:*:19873:0:99999:7:::
sync:*:19873:0:99999:7:::
games:*:19873:0:99999:7:::
man:*:19873:0:99999:7:::
lp:*:19873:0:99999:7:::
mail:*:19873:0:99999:7:::
news:*:19873:0:99999:7:::
uucp:*:19873:0:99999:7:::
proxy:*:19873:0:99999:7:::
www-data:*:19873:0:99999:7:::
backup:*:19873:0:99999:7:::
list:*:19873:0:99999:7:::
irc:*:19873:0:99999:7:::
gnats:*:19873:0:99999:7:::
nobody:*:19873:0:99999:7:::
_apt:*:19873:0:99999:7:::
hacker::20000:0:99999:7:::
zardus:$6$AUgCQbqjJYZCvnNE$sjSTi51IMFOewF8YWTKNBeEnUIdbo2KaxJOm.BwjuAimnwdTFA/49720RkIbuoeuORZ27EXLgPV9YG/PC3edi0:20015:0:99999:7:::
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:20 100% 2/3 0.04909g/s 285.8p/s 285.8c/s 285.8C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{cBSSdtSjQnUALsVBmpyHPWhaX_E.ddTN0UDL4gjN0czW}
```
