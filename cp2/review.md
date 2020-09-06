R1: 

Web - HTTP

email -> SMTP\POP3\IMAP

FTP -> FTP

R2:

网络体系结构是固定的，并未应用程序提供特定的服务集合。应用程序结构主要有两种：

- 客户-服务器体系

- 对等体系结构 P2P

R3:

对于 Web 而言，浏览器是客户，服务器进程是服务器。在不同应用中客户和服务器有所不同，在有些应用者，它既可能是客户又可能是服务器，比如CDN。

R4:

不同意。

R5:

IP 地址和端口号。

R6:

UDP，虽然UDP 是 unreliable 的，但是它不是建立在连接的基础上，不需要握手阶段，因此会更快。

R7:

IM 应用？多人游戏应用？

R8:

运输层主要提供如下四种宽泛的服务；

1. 可靠的数据传输（TCP）

2. 吞吐量（运输协议没有提供）

3. 定时（运输协议没有提供）

4. 安全性(SSL ，但是 SSL 不属于运输层协议)

R9:

属于应用层协议。

R10:

握手的作用是确保建立连接，保证后面的数据通信和传输。

R11:

因为他们都需要确保数据准备可靠的传输。

R12:

主要分为四个步骤：

- 首先服务端会判断是否带有 cookie，没有就添加一个 set-cookie 的 response header。

- set-cookie 会将会话 cookie 保存在浏览器端，之后每次向服务端请求都会带上之前设置的 cookie

- 服务端根据 request header 来跟踪用户的状态

- 客户端的 cookie 是通过浏览器来维护的，服务端的 cookie 信息保存在数据库中。

R13:

首先当我们请求一个 object 时，我们是想 web cache server 发送请求，如果该 cache server 没有请求的对象，那么 cache server 就会想 origin server 发送请求，来拉去请求对象，这个过程被称作回源，同时 cache server 会将请求回来的 object 保存下来，并将 object 返回给 client，当 client 再次发起相同请求的时候，cache server 就直接将缓存下来的 object 返回给 client了。而不用再次向 origin server 发送请求，也就相应的减少了请求时间。

Web cache server 应该是减少了所有对象的请求时延，包括 html、js、css、图片等。

R14:

略

R15:

因为 FTP 有两个 TCP 链接，分别是 control connection 和 data connection。control connection 主要控制授权、登录、文件操作。data connection 主要是传递文件。因此FTP 是带外传递控制信息。

R16:

Alice 首先通过 HTTP 协议将 报文发送到 Alice 的邮件服务器，Alice 的邮件服务器通过 SMTP 协议将邮件内容发送到 Bob 的邮件服务器，Bob 邮件服务器将 Alice 发送的邮件投递到 Bob 的 email box 中，最后，Bob 通过 POP3 协议来拉去 Alice 发送的邮件内容。

R17:

问题是 HTTP 协议的 首部吗？

R18:

不知道

R19:

可以，MX。

R20:

略。


