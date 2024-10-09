# Redirecting input

First I used the `echo` command and redirected its output to the `PWN` file using the `>` operator.
Then I redirected the input of the `PWN` file into `/challenge/run` using the `<` operator, which gave me the flag `pwn.college{4iqlH5T6AxoDEgazADfLlzhehQS.dBzN1QDL4gjN0czW}`

```bash
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{4iqlH5T6AxoDEgazADfLlzhehQS.dBzN1QDL4gjN0czW}
```
