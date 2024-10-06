# An Epic Filesystem Quest

First went to the `/` directory using `cd` command then used `ls-a` to find list the files(even the hidden ones) then went on to find the `HINT` file.
Then I used the `cat` command to read the `HINT` file which pointed me to `/opt/linux/linux-5.4/arch/x86/kernel/fpu` however since I was told that I couldn't `cd` into the directory without triggering a trap, I instead used `ls` and `cat` commands to view and read the `ALERT-TRAPPED` file. Which gave me the next clue.
Then I used `ls -a` to reveal hidden files in the directory `/opt/linux/linux-5.4/drivers/net/ethernet/hisilicon` which lead me to the `.MEMO` file which gave the next clue.
Then I navigated to a new directory using `cd` where the clue would only be accessible after entering the directory. After cding into `/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm`, I listed the files using `ls- a` and read the `POINTER` file using the `cat` command to get the next clue.
Then I used the `ls -a` again to reveal another hidden file, `.MESSAGE`, which gave the next directory to search.
Then because of searching the directory I found a file named `WHISPER` and read it, which directed me to another directory.
Then I retrieved the next clue by reading `TIP-TRAPPED` without entering the directory, using `ls-a` and `cat` without using `cd`,avoiding another trap.
After navigating to the next directory, I found the `DISPATCH file`, which provided another clue.
Finally, after following all the clues, I found the `INFO` file in the `/opt/linux/linux-5.4/Documentation/features/vm/PG_uncached` directory, which contained the flag `pwn.college{AtIJq280Awacr0QRmz5A99cXPbt.dljM4QDL4gjN0czW}`

```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls -a
.   .dockerenv  bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
..  HINT        boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@commands~an-epic-filesystem-quest:/$ cat HINT
Tubular find!
The next clue is in: /opt/linux/linux-5.4/arch/x86/kernel/fpu

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/$ ls /opt/linux/linux-5.4/arch/x86/kernel/fpu
ALERT-TRAPPED  bugs.c  built-in.a  core.o  init.o    regset.o  signal.o  xstate.o
Makefile       bugs.o  core.c      init.c  regset.c  signal.c  xstate.c
hacker@commands~an-epic-filesystem-quest:/$ cat /opt/linux/linux-5.4/arch/x86/kernel/fpu/ALERT-TRAPPED
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/drivers/net/ethernet/hisilicon

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ ls -a /opt/linux/linux-5.4/drivers/net/ethernet/hisilicon
.  ..  .MEMO  Kconfig  Makefile  hip04_eth.c  hisi_femac.c  hix5hd2_gmac.c  hns  hns3  hns_mdio.c
hacker@commands~an-epic-filesystem-quest:/$ cat /opt/linux/linux-5.4/drivers/net/ethernet/hisilicon/MEMO
cat: /opt/linux/linux-5.4/drivers/net/ethernet/hisilicon/MEMO: No such file or directory
hacker@commands~an-epic-filesystem-quest:/$ cat /opt/linux/linux-5.4/drivers/net/ethernet/hisilicon/.MEMO
Tubular find!
The next clue is in: /opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ ls -a
.   POINTER     meson.build  signal.c    syscall.tbl    target_cpu.h  target_fcntl.h   target_structs.h  termbits.h
..  cpu_loop.c  nwfpe        sockbits.h  syscallhdr.sh  target_elf.h  target_signal.h  target_syscall.h
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ cat POINTER
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/include/config/x86/pkg

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ ls -a /opt/linux/linux-5.4/include/config/x86/pkg
.  ..  .MESSAGE  temp
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ cat /opt/linux/linux-5.4/include/config/x86/pkg/.MESSAGE
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/arch/arm/plat-pxa
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ ls -a /opt/linux/linux-5.4/arch/arm/plat-pxa
.  ..  Kconfig  Makefile  WHISPER  include  mfp.c  ssp.c
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ cat /opt/linux/linux-5.4/arch/arm/plat-pxa/WHISPER
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/tools/testing/scatterlist/linux

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ ls -a /opt/linux/linux-5.4/tools/testing/scatterlist/linux
.  ..  TIP-TRAPPED  mm.h
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ cat /opt/linux/linux-5.4/tools/testing/scatterlist/linux/TIP-TRAPPED
Congratulations, you found the clue!
The next clue is in: /usr/share/racket/pkgs/games/paint-by-numbers/compiled
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ ls -a /usr/share/racket/pkgs
/games/paint-by-numbers/compiled
.         all-problems_rkt.dep  gui_rkt.zo    paint-by-numbers_rkt.dep  problem_rkt.zo
..        all-problems_rkt.zo   info_rkt.dep  paint-by-numbers_rkt.zo   solve_rkt.dep
DISPATCH  gui_rkt.dep           info_rkt.zo   problem_rkt.dep           solve_rkt.zo
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ cat /usr/share/racket/pkgs/games/paint-by-numbers/compiled/DISPATCH
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/Documentation/features/vm/PG_uncached
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ ls -a /opt/linux/linux-5.4/Documentation/features/vm/PG_uncached
.  ..  INFO  arch-support.txt
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/linux-user/arm$ cat /opt/linux/linux-5.4/Documentation/features/vm/PG_uncached/INFO
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{AtIJq280Awacr0QRmz5A99cXPbt.dljM4QDL4gjN0czW}
```
