# Reading Manuals
Used the `man` command to display the manual of a command. Here I used `man challenge` making `challenge` as an argument. Then read about `--ucpiwd NUM` used as argument for the `challenge` will print the flag if the `NUM` is `084`.Using that I got the flag `pwn.college{0FCuIcp-iWw8VEd4cSuWkfpA0TW.dRTM4QDL4gjN0czW}`
```bash
hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)                                      Challenge Commands                                     CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --ucpiwd NUM
              print the flag if NUM is 084

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)
hacker@man~reading-manuals:~$ /challenge/challenge --ucpiwd 084
Correct usage! Your flag: pwn.college{0FCuIcp-iWw8VEd4cSuWkfpA0TW.dRTM4QDL4gjN0czW}
```
