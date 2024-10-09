# Printing Variables

Here I learned that we can use the `$` sign before a variable in combination with the `echo` command to print out the value of the variable instead of the variable name itself.
First I used `echo` command with `$FLAG`, where `FLAG` is a variable holding the value `pwn.college{0GIOxu_vY6HhX2dpbgdcUAWq3vE.ddTN1QDL4gjN0czW}`. Because of the `$` sign it printed the value of the `FLAG` variable

```bash
hacker@variables~printing-variables:~$ echo $FLAG
pwn.college{0GIOxu_vY6HhX2dpbgdcUAWq3vE.ddTN1QDL4gjN0czW}
```
