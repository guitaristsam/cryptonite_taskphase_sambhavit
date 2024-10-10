# Exporting Variables

Here I learned that I can export a variable using the `export` command.
Using this to satisfy the conditions of the `PWN` variable being set to the value of `COLLEGE` and it being exported using `export PWN=COLLEGE`
and `COLLEGE` variable being set to the value of `PWN` but not being exported using `COLLEGE=PWN`. Using this I got the flag `pwn.college{4D0EccLu9D83Gj-zQumIhmcXeo1.dJjN1QDL4gjN0czW}`

```bash
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{4D0EccLu9D83Gj-zQumIhmcXeo1.dJjN1QDL4gjN0czW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```
