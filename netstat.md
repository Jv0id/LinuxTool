netstat
======
它可以打印本地网卡接口上的全部连接、路由表信息、网卡接口信息等。我们一般使用它的第一个功能，对于后两者功能我们可以采用更强大的`route`和`ifconfig`来查看。
##常用选项
|选项|描述
|:--:|---
|-n|使用IP表示主机，而不是主机名；使用数字表示端口，而不是服务名
|-a|显示所有socket，包含监听socket
|-l|仅显示监听socket
|-t|仅显示TCP连接
|-r|显示路由信息
|-i|显示网卡接口的数据流量
|-c|每隔1s输出一次
|-o|显示socket定时器的信息
|-p|显示socket所属进程的PID和名字

加不加`-n`所打印的信息数量是一样的，只不过缺省情况下会用主机名（比如域名）来表示主机，如果加了`-n`，则用IP地址表示主机。没有主机名的一律都是IP地址显示。  
另外，缺省的情况下不显示监听socket。