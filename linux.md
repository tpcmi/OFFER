# IO多路复用

通过某种机制让单个进程可以监视多个文件描述符，一旦某个描述符就绪，能通知程序进行相应的读写操作

socket创建的套接字默认都是阻塞的，线程一直处于等待状态，直至操作完成获得结果或者超时出错

阻塞模式的套接字编程简单，但是在服务器端通常要处理大量套接字通信请求，当线程阻塞而无法处理其他运算或响应请求，效率低下；采用多线程会占用很大内存空间，且线程切换会有很大开销

![preview](https://pic2.zhimg.com/v2-e6a869884585625dfc7eace1b90c3024_r.jpg)

## select

由于fd_set是一个bitmap位图结构，默认最大监听数量为1024，当有文件就绪时，会设置为1，并返回select

poll

epoll



## vim

[An adventure game](https://vim-adventures.com/)



## g++、gcc

