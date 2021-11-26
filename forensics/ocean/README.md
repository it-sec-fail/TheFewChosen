# OCEAN
What can you do in an ocean of files?

[nc server.challenge.ctf.thefewchosen.com 1338](nc server.challenge.ctf.thefewchosen.com 1338)

There is an official hint: 

> Hint for ocean:
> The chal file is not relevant. That's just a shell (basically the entrypoint). Try listing folders and subfolders

So we looked around for a while and found this directory (Magic trick was to use ls -R instead of find):

```shell
pwd
/usr/bin/what
ls -tr
0.T
1.F
2.C
3.C
4.T
5.F
6.{
7.J
8.u
9.5
10.t
11._
12.k
13.3
14.3
15.p
16._
17.5
18.w
19.1
20.m
21.m
22.1
23.n
24.g
25.}
```

So this is the flag:

> TFCCTF{Ju5t_k33p_5w1mm1ng}
