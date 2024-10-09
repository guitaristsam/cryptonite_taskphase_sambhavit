# implicit relative path

Used a relative path of `./run` instead of `./challenge/run` because it is an implicit relative path,
First changed current directory to `challenge` using the `cd` command then ran `./run` to find flag `pwn.college{4eNDo3oD-_7NKr4PJxf0gJzgUqQ.dFTN1QDL4gjN0czW}`

```bash
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{4eNDo3oD-_7NKr4PJxf0gJzgUqQ.dFTN1QDL4gjN0czW}
```
