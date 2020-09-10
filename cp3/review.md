R1:

a.我们将这个协议取名为 Simple Transfer Protocol，它从应用层拿到数据，和IP地址、端口号，将数据拆分成不同的 thunks，然后给每一个 thunk 添加一个 header，将端口号放到 header 中，然后将 IP 地址和封装好的 thunks 交给网络层，网络层将 thunks 传递到目的主机的网络层，然后递交给目的主机的运输层，目的主机的运输层从thunks 中提取出端口号，并且组装成完整数据，根据目的端口号，交给相应的进程。

b.应用层就需要将源IP，源 port 和目的 ip 目的 port 都给运输层，然后运输层的header 包含 两个 port，然后将 两个 ip 及 thunks 传给给网络层，其它基本都一样。

c. 不是，Translation layer 在端系统中。

R2:

a. 在这个过程中，家庭成员之一扮演的就是运输层的工作，在发件方，家庭代表成员将发件人的姓名写在了信件的顶部，然后塞进信封，交给邮递员，邮递员运输改信件到目的家庭，目的家庭的代表成员打开信封，找到收件人，然后将信件交到收件人手里。

b.不需要

R3:

source port is y and destination port is x。

R4:

应为 UDP 不需要建立连接，因此传输效率会更高。同时 TCP 拥有流量控制和拥塞控制，而 UDP 没有，所以 UDP 可以以更快的速率传输。

R5:

因为大部分的防火墙都会阻碍 UDP 流量。

R6:

可以，需要应用程序自己实现可靠的数据传输。

R7:

是的，在报文中有 source id 和 port。

R8:

不是相同的 Socket，都是 80 端口号，不同的 Socket 通过 源 ip，port 和 目的 ip、port 来识别。
