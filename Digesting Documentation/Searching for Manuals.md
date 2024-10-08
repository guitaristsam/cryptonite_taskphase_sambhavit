# Searching for Manuals

First used `man man` to read manual for the command `man` which showed me that I can use `man -k` to search for keywords. I used this to search for challenge using `man -k challenge` then I got `cjxbinxrdg (1)       - print the flag!`.
Using that I did `man cjxbinxrdg` to find `--cjxbin NUM` and got to know that it would print the flag if the `NUM = 164`.Then I ran `/challenge/challenge --cjxbin 164` to get the flag `pwn.college{M16KcjXLJxP-VbBEinQxrXUTRJS.dZTM4QDL4gjN0czW}`

```bash
hacker@man~searching-for-manuals:~$ man man
MAN(1)                                            Manual pager utils                                           MAN(1)

NAME
       man - an interface to the system reference manuals

SYNOPSIS
       man [man options] [[section] page ...] ...
       man -k [apropos options] regexp ...
       man -K [man options] [section] term ...
       man -f [whatis options] page ...
       man -l [man options] file ...
       man -w|-W [man options] page ...

DESCRIPTION
       man  is the system's manual pager.  Each page argument given to man is normally the name of a program, utility
       or function.  The manual page associated with each of these arguments is then found and displayed.  A section,
       if  provided,  will direct man to look only in that section of the manual.  The default action is to search in
       all of the available sections following a pre-defined order (see DEFAULTS), and to show only  the  first  page
       found, even if page exists in several sections.

       The table below shows the section numbers of the manual followed by the types of pages they contain.

       1   Executable programs or shell commands
       2   System calls (functions provided by the kernel)
       3   Library calls (functions within program libraries)
       4   Special files (usually found in /dev)
       5   File formats and conventions, e.g. /etc/passwd
       6   Games
       7   Miscellaneous (including macro packages and conventions), e.g. man(7), groff(7)
       8   System administration commands (usually only for root)
hacker@man~searching-for-manuals:~$ man -k challenge
cjxbinxrdg (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man cjxbinxrdg

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

       --cjxbin NUM
              print the flag if NUM is 164

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)
hacker@man~searching-for-manuals:~$ /challenge/challenge --cjxbin 164
Correct usage! Your flag: pwn.college{M16KcjXLJxP-VbBEinQxrXUTRJS.dZTM4QDL4gjN0czW}
```
