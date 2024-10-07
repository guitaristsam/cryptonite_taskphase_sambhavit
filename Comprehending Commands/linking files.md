# linking files
Here I made a symbolic link using `ln -s` then I ran the challenge program again to read from `not-the-flag`, which is now pointing to `/flag`.
flag: `pwn.college{87W3kWs6dldShkKYiVIXwM2l0Vk.dlTM1UDL4gjN0czW}`
```bash
ln -s /flag not-the-flag
/challenge/catflag
```
