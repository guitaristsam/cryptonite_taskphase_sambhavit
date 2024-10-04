# hidden files

First, I navigated to the `/` directory using the `cd` command, then used `ls -a` to list all files, including hidden ones, and then used cat to display the contents of the hidden flag file,`.flag-318023150924405`

```bash
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-318023150924405  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-318023150924405
pwn.college{YhAvM6_eRfzrF7zwfXUdKYcqfXx.dBTN4QDL4gjN0czW}
```
