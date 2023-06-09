# 谷歌想用它的 QUIC 协议 加速网络

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/04/18/google-wants-to-speed-up-the-web-with-its-quic-protocol/>

你可能从未听说过它，但如果你是 Chrome 用户，你可能已经使用过谷歌的 QUIC 协议了。正如谷歌本周披露的，Chrome 向谷歌服务器发出的所有请求中，约有一半是通过 QUIC 服务的。

这有什么大不了的？QUIC 是谷歌在 UDP 上的实验性低延迟互联网传输协议，这是一种经常被游戏、流媒体和 VoIP 服务使用的协议。名称“QUIC”代表快速 UDP 互联网连接。

UDP(和 QUIC)在协议世界中的对应物基本上是 TCP(它与互联网协议(IP)一起构成了互联网的核心通信语言)。UDP 明显比 TCP 更轻量级，但反过来，它的纠错服务比 TCP 少得多。例如，这意味着发送服务器不会经常与接收服务器通信来检查包是否到达以及它们是否以正确的顺序到达。这就是为什么 UDP 非常适合游戏服务的原因。对于这些服务，您希望低开销以减少延迟，如果服务器没有接收到您最近的鼠标移动，没有必要花一两秒钟来修复它，因为动作已经继续了。不过，你不会想用它来请求一个网站，因为你不能保证所有的数据都会成功。

通过 QUIC，Google 旨在将 UDP 和 TCP 的一些最佳特性与现代安全工具相结合。

![0rtt-graphic](img/cd26f5d011f8c74c75ef715bf0847380.png)

在典型的安全 TCP 连接中，浏览器通常需要两到三次往返才能真正开始接收数据。使用 QUIC，一个浏览器可以立即开始与一个它以前对话过的服务器对话。QUIC 还引入了一些新功能，如拥塞控制和自动重传，使它比纯 UDP 更可靠。

通过后来成为 HTTP/2 标准基础的 SPDY，Google 已经开发了另一种替代协议，它与 QUIC 有许多相同的目标，但是 HTTP/2 仍然运行在 TCP 之上，并且仍然会遇到一些相同的延迟成本。

有理由问为什么 Google 不仅仅致力于改进 TCP。该公司[指出](https://web.archive.org/web/20230330130256/https://docs.google.com/document/d/1lmL9EF6qKrk7gbazY8bIdvq3Pno2Xj_l_YShP40GLQE/edit)这里的问题是，TCP 支持通常直接内置在操作系统内核中——这不是谷歌可以控制的。该团队在解释其决定时写道:“QUIC 允许我们测试和试验新的想法，并更快地获得结果。”。“我们希望，如果证明有效，QUIC 特性将移植到 TCP 和 TLS 中。”鉴于目前仍有多少 Windows XP 安装，这显然不是一朝一夕的事情。

如果谷歌设计了一个全新的协议，那么构成互联网主干的所有机器也必须理解它——但它们已经理解了 UDP。

![2015-04-18_1036](img/7d738be0651d106a754c4810e6ea0c60.png)谷歌表示，在谷歌搜索上使用 QUIC 后，平均页面加载时间提高了约 3%。这听起来不是很多，但你必须记住，谷歌搜索已经尽可能优化。其他网站——尤其是延迟严重的网络应用——可能会有更好的改进。通过 QUIC 连接到 YouTube 的用户报告说，观看视频时的重新缓冲减少了大约 30 %,由于 QUIC 通过 UDP 改进了拥塞控制和丢失恢复，一些最慢连接的用户也可以通过 QUIC 缩短页面加载时间。

谷歌表示，它计划向 IETF 提出 HTTP2-over-QUIC 作为未来新的互联网标准。

在某些方面，这反映了谷歌与 [SPDY](https://web.archive.org/web/20230330130256/https://en.wikipedia.org/wiki/SPDY) 的合作。在那里，该公司首先使用 Chrome 和自己的服务器制作了协议原型，后来又提出将其作为新版 HTTP 的基础。

如果你想看看你与 Chrome 的连接是否使用 QUIC，顺便说一下，[这里有一个浏览器扩展](https://web.archive.org/web/20230330130256/https://chrome.google.com/webstore/detail/http2-and-spdy-indicator/mpbpobfflnpcgagjijhmgnchggcjblin?hl=en)可以告诉你，你可以在 *net-internals 标志*(Chrome://net-internals/# QUIC)下找到关于 Chrome 使用 QUIC 的所有细节。