# 最新的斯诺登爆料揭露了美国国家安全局的监听范围 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/12/29/latest-snowden-revelations-expose-scope-of-nsa-interceptions/>

上周末，[德国新闻媒体 Spiegel 发表了一篇关于美国国家安全局破解加密通信形式能力的报道](https://web.archive.org/web/20221207050211/http://www.spiegel.de/international/germany/inside-the-nsa-s-war-on-internet-security-a-1010361.html)，揭露了该机构对网络服务器用来传输敏感信息的 SSL/TLS 的例行拦截。该报告还揭露了一个事实，即该机构有能力解密虚拟专用网络。

但或许更重要的是，从爱德华·斯诺登(Edward Snowden)泄露的大量文件中精选出来的信息显示了美国国家安全局难以破解的加密形式(至少在 2012 年文件泄露时是如此)。该清单包括 PGP、Tor、CSpace、OTR 和 ZRTP。

好消息和坏消息的结合获得了相互矛盾的报道， [The Verge](https://web.archive.org/web/20221207050211/http://www.theverge.com/2014/12/28/7458159/encryption-standards-the-nsa-cant-crack-pgp-tor-otr-snowden) 强调了美国国家安全局无法攻破的网络， [Slashdot](https://web.archive.org/web/20221207050211/http://yro.slashdot.org/story/14/12/28/2054228/snowden-documents-show-how-well-nsa-codebreakers-can-pry) 以“斯诺登文件显示了美国国家安全局解密者可以窥探得多好”为标题

总的来说，这份报告令人放心。自斯诺登文件公开以来的 18 个月里，那些担心安全的人采取的许多形式的附加加密措施都是有效的。例如，文件显示，受 ZRTP 保护的通信(RedPhone 使用的加密类型)阻止了 NSA。

“很高兴知道美国国家安全局认为我们应用程序的加密通信是真正不透明的，”RedPhone 开发者莫邪·马林斯派克告诉《明镜》周刊。

虽然 SSL 和 VPN 连接上的拦截范围令人担忧，但许多人认为该机构以前拥有这种能力。Spiegel 公布的资料显示了该机构在这方面使用的具体工具。

《明镜》的报道在信息安全界引发了强烈反对，一些人说它耸人听闻地夸大了美国国家安全局通过 VPN 连接获取信息的能力。根据 Spiegel 的说法，美国国家安全局运营着“一个大规模的 VPN 开发项目，以破解大量连接，使其能够拦截 VPN 内部的数据——例如，包括希腊政府对 VPN 的使用。”

这是一个非常令人担忧的发现，考虑到大量的公司和政府利用 VPN 允许用户在世界任何地方访问他们的网络。但是安全专家博客 No Hats 称，如果你正确配置你的 VPN，你不会受到影响。根据 Spiegel 报告所依据的博客对 NSA 幻灯片的综合分析，正确配置的基于 IPsec 的 VPN 是没问题的。

这篇文章中另一个令人担忧的统计数据是该机构截获的 https 连接的数量，这是脸书等网站使用的安全连接类型。一份文件显示，到 2012 年底，美国国家安全局每天破解 1000 万个这样的连接。

《明镜》周刊的文章大部分讨论了美国国家安全局面临的利益冲突:它负责推荐安全标准，但却不断试图打破它所推荐的安全标准。

乍一看，这些说法似乎指向了我们一次又一次被提醒的伪善，因为更多的美国监控国家被揭露出来。隐私倡导者普遍认为，易受执法机构攻击的通信也面临各种网络威胁，从试图窃取身份的罪犯到外国政府的黑客。似乎违反直觉的是，NSA 将负责建立它只想打破的标准，特别是当[美国执法机构有一个历史](https://web.archive.org/web/20221207050211/http://www.wsj.com/articles/fbi-chief-warns-phone-encryption-may-have-gone-too-far-1413489352)希望通信不那么安全，以使获取信息更容易。

但是在[的一篇批评《明镜》报道](https://web.archive.org/web/20221207050211/http://blog.erratasec.com/2014/12/that-spiegel-nsa-story-is-nonsense.html#.VKGFRMACw)的博客文章中，网络安全专家 Robert Graham 称其为“激进分子的胡说八道”，称 NSA 试图打破其设定的标准是一件好事。

他写道:“你通过试图破坏来保护事物。”。

《明镜》周刊的报道泄露了大量文件，这些文件包含了有关美国国家安全局技术的非常具体的信息。在《卫报》和《华盛顿邮报》首次公布文件一年半后，该报告再次引发了社交媒体上要求全面公布斯诺登文件的呼声。如果有什么不同的话，这份报告提醒我们，美国的监控行为可能会有多年的新曝光。