#select_TcpIp


CLient:
In here, we have some problem like:
1. if we get eof from socket, we cannnot make sure
what happen in here.
2. we also get some buffer problem.

But if we use select, it will not have those problems.
We can use select to monitor which part get eof status.

Server:
In the previous program, we use muti-process. But if we
get lots of client, the cpu can not create much processes
like thousands. So in this program, we use select to handle
this. Each process can handle 1024 fp.






