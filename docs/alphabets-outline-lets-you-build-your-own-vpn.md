# 字母表的轮廓让您可以构建自己的虚拟专用网络

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/03/22/alphabets-outline-lets-you-build-your-own-vpn/>

字母表的网络安全部门 [拼图](https://web.archive.org/web/20221007230829/https://jigsaw.google.com/)发布了一个有趣的新项目，名为[提纲](https://web.archive.org/web/20221007230829/https://getoutline.org/)。如果我把事情简化很多，它允许任何人在 DigitalOcean 上创建并运行一个 VPN 服务器，然后授予您的团队访问该服务器的权限。

我玩了一会儿《大纲》,这是一个有趣的产品。有两个组件，一个管理应用程序和一个客户端。让我们从经理开始。

现在，该管理器在 Windows 和 Linux 上可用，很快就会有一个 macOS 版本。这是一个电子应用程序，所以感觉像是在使用一个网络应用程序。默认情况下，Outline 建议您使用著名的云托管提供商 [DigitalOcean](https://web.archive.org/web/20221007230829/https://www.digitalocean.com/) 。

您也可以在另一台服务器上创建您的虚拟专用网服务器，但这并不是要点。大纲是关于尽可能容易地运行您自己的服务器。否则您已经在使用 [Algo VPN](https://web.archive.org/web/20221007230829/https://github.com/trailofbits/algo) 或[史翠珊](https://web.archive.org/web/20221007230829/https://github.com/StreisandEffect/streisand)。

如果您选择数字海洋，该应用程序会打开一个网络视图，并要求您输入登录名、密码和一次性密码。之后，您需要让 Outline 使用 DigitalOcean API。这就是您在初始设置过程中需要做的全部工作。

现在，让我们创建一个虚拟专用网服务器。大纲自动选择 DigitalOcean 上最便宜的液滴，1TB 的传输数据每月需要 5 美元(不知何故，大纲说您可以得到 500GB)。数字海洋目前在 8 个不同的城市拥有数据中心——阿姆斯特丹、新加坡、班加罗尔、法兰克福、伦敦、旧金山、多伦多和纽约。

选择一个城市后，管理应用程序会自动下载[一个码头工人图像](https://web.archive.org/web/20221007230829/https://quay.io/repository/outline/shadowbox?tab=tags)，并基于该码头工人图像在数字海洋上创建一个服务器。服务器上的软件将每小时自动更新一次。您的 DigitalOcean 服务器也将自动执行操作系统的安全更新，并在必要时重新启动服务器。

![](img/e7383166a97fb7afa844d24a18c897b9.png)

现在让我们回到你现在使用的电脑。现在，您可以从管理应用程序控制您的 VPN 服务器。默认情况下，Outline 只为您生成一个键。但是您可以添加更多用户并邀请您的同事使用您的服务器。

如果用户不再需要访问您的服务器，您可以使用管理应用程序来创建更多服务器、删除服务器或删除用户。该应用程序还会告诉你每个用户使用了多少带宽。

邀请页面只是亚马逊 S3 上的一个静态网页，有两个东西。首先，该页面邀请您在手机或计算机上下载 Outline 客户端。第二，关键在网址。当您加载页面时，浏览器会显示密钥。

这就是为什么你不应该用不加密的方法邀请你的朋友——不要用脸书，不要用电子邮件。请记住，密钥也将存储在您的浏览器历史记录中。

但是连接到 VPN 服务器就像安装一个应用程序和点击一个邀请链接一样简单。对于不懂技术的用户来说，这是一个很好的体验。

让我们谈一下客户。您用来连接 VPN 服务器的应用程序目前在 Windows、Android 和 Chrome 操作系统上可用。Jigsaw 正在 macOS 和 iOS 客户端上工作。它的特点是一个单一的屏幕，让您连接和断开服务器-非常简单。

## 大纲不是 VPN

在引擎盖下，大纲依赖于[影子袜子](https://web.archive.org/web/20221007230829/https://en.wikipedia.org/wiki/Shadowsocks)协议。如果你熟悉 VPN 协议，Shadowsocks 与 OpenVPN、IPSec 或 WireGuard 完全不同。事实上，Shadowsocks 根本不是一个 VPN 协议。

Shadowsocks 是一个开源项目，用于创建加密的 socks5 代理来重定向互联网流量。这有点技术性，但是 VPN 就像是你的设备和服务器之间的加密隧道。你所有的网络流量都通过这个隧道，VPN 服务器(不是你的手机或电脑)是连接互联网的设备。

它很棒，因为你可以肯定地知道，你的 ISP 和你的 WiFi 网络上的其他用户无法查看你的流量(除非有 DNS 泄漏)。你也可以假装你在另一个国家。

但这也很糟糕，因为任何能访问你的 VPN 服务器的人都能看到你的网络流量。这就是为什么你应该*永远不要*依赖 VPN 公司，即使他们承诺尊重你的隐私。他们会分析你的浏览习惯，卖给广告商，在不安全的页面上注入他们自己的广告或者窃取你的身份。你也不能确定是否可以信任他们。

传统的 VPN 协议也可能被阻止，因为它们使用特定的端口，如果权威机构和 ISP 使用深度数据包检测，它们看起来就像 VPN 流量。这就是为什么各国可以完全屏蔽 VPN。

然而，socks5 代理看起来像正常的互联网流量。Shadowsocks 正在利用这一点，并将代理的优势与流量加密相结合。举例来说，它在中国应该很管用。

但你不能保证所有的互联网流量都通过代理服务器——这取决于每个应用程序。代理增加了粒度级别，这可能很方便，但也是一个安全问题。例如，Outline 客户端不会立即将所有 Windows 流量重定向到 Outline 服务器。

所以，如果你想用你的网络浏览器访问被审查的网站，Outline 可能是一个完美的工具。但是你不会因为一个大纲连接就从网络上消失。

![](img/7f49b96126711992585165dece4de359.png)

## 信任谷歌

很难忘记《大纲》是一个拼图项目。从事这个项目的人由谷歌的母公司 Alphabet 支付工资。换句话说，当涉及隐私时，很难相信谷歌的项目。

但是竖锯真的希望你相信他们。大纲是一个[开源项目](https://web.archive.org/web/20221007230829/https://github.com/Jigsaw-Code/outline-server)。这样，专家就可以查看代码，看看是否有什么可疑之处。这项服务已经由第三方安全公司[在](https://web.archive.org/web/20221007230829/https://s3.amazonaws.com/outline-vpn/static_downloads/ros-report.pdf)进行了审计。

Jigsaw [收集带有不可识别数据的崩溃日志](https://web.archive.org/web/20221007230829/https://s3.amazonaws.com/outline-vpn/index.html#/en/support/dataCollection)。他们还收集所有服务器 IP，但无法访问那些服务器——我不确定 Jigsaw 为什么要查看所有 IP。您也可以选择分享更多使用数据。

你的概要服务器不记录你的网络流量。因此，即使国家安全局有进入一个大纲服务器的授权，它也只能找出每个用户使用这个服务器的带宽。但是没有办法把这些点联系起来，找出谁是这个大纲服务器的幕后黑手。

最大的风险可能是数字海洋。你必须输入你的名字，电子邮件和信用卡来创建一个数字海洋账户。当局可以要求 DigitalOcean 找出谁在为你的服务器买单，然后给你回复。

## 安全性与可访问性

Outline 并不是最安全的 VPN。最好是建立自己的硬件服务器，使用不用自己付费的连接方式连接到互联网，并自己安装 VPN 软件。

但是没有人会这么做。

隐私总是安全性和可访问性之间的平衡。最安全的工具也是最难使用的工具。

许多项目现在正试图使安全性更容易实现。这是一股清新的空气。Algo VPN 让你[只用几个命令行就能构建自己的 IPSec VPN 服务器](https://web.archive.org/web/20221007230829/https://techcrunch.com/2017/04/09/how-i-made-my-own-vpn-server-in-15-minutes/)。[史翠珊](https://web.archive.org/web/20221007230829/https://github.com/StreisandEffect/streisand)也可以让你用很少的技术知识建立一个有各种协议的服务器。

这些都是很棒的项目，如果你想建立自己的 VPN，我建议你看看它们。但是大纲更进了一步。创建 Shadowsocks 服务器不需要输入任何命令行。

Jigsaw 说这是新闻机构的完美工具。的确，大多数记者都知道如何安装应用程序。没有加 VPN 证书那么恐怖。我会说，如果你住在中国或其他有限制的国家，即使你不是记者，这也是访问审查网站的好方法。

你必须评估你的风险水平，选择适合你的技术解决方案。如果你没有做任何违法的事情，只是想访问被屏蔽的网站，你可以做出一些让步。

有一点是肯定的，Outline 比任何免费或商业 VPN 服务都要好。

![](img/7754ddb659fd640a4c00c49410fba822.png)