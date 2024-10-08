# Matching paths with [ ]

Here I ran `/challenge/run` with the argument `/challenge/files/file_[bash]` which satisfies the conditon by expanding to `/challenge/files/file_b`, `/challenge/files/file_a`, `/challenge/files/file_s`, `/challenge/files/file_h` and giving the flag `pwn.college{00m7nQEjXD3zWWlCv-LEvBNGQ6A.dRjM4QDL4gjN0czW}`

```bash
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{00m7nQEjXD3zWWlCv-LEvBNGQ6A.dRjM4QDL4gjN0czW}
```
