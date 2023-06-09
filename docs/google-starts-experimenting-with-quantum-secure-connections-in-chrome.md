# 谷歌开始在 Chrome TechCrunch 中试验量子安全连接

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/07/07/google-starts-experimenting-with-quantum-secure-connections-in-chrome/>

# 谷歌开始在 Chrome 中试验量子安全连接

如果量子计算实现了它的承诺(在现阶段这仍然是一个很大的“如果”)，有人可以使用这项技术追溯破解任何用今天的标准加密算法加密的通信。为了防止这种情况，谷歌今天宣布，它将开始使用后量子算法对实验性的 T2 金丝雀版本的 Chrome 和它的一些服务之间的连接进行加密。

需要说明的是，目前这只是一个实验，只有一小部分浏览器和谷歌服务器之间的连接会使用这种新算法。

然而，这里的想法是将这个想法带到最前沿，并“获得后量子算法可能需要的更大数据结构的真实世界经验，”谷歌工程师[马特·布莱斯维特](https://web.archive.org/web/20221208230552/https://www.linkedin.com/in/asdfasdfsadfsadfasdfasdf)在今天的公告中写道。

很少有人完全理解量子计算，更不用说量子密码了。不过，据我所知，除了这种新的后量子密钥交换算法之外，新系统还将使用标准加密技术。具体来说，该团队正在使用 [*新希望*算法](https://web.archive.org/web/20221208230552/https://eprint.iacr.org/2015/1092.pdf)，该算法旨在为 TLS 提供后量子安全——使 HTTPS 安全的协议。

拥有发布新互联网协议历史的谷歌明确表示，它不想创建一个新的事实标准。布莱斯维特指出*新希望*是该团队在 2015 年 12 月调查这个项目时发现的最有前途的后量子密钥交换。然而，自那以后，该领域的更多研究已经发表——包括来自与恩智浦、微软、Centrum wisk unde&Informatica 和麦克马斯特大学合作的[谷歌研究人员团队的研究。正因为如此，谷歌计划在两年内停止目前的实验。](https://web.archive.org/web/20221208230552/https://eprint.iacr.org/2016/659)

如果你想参与实验，你必须安装 Chrome 的金丝雀版本[(有时可能不稳定)，如果运气好的话，偶尔连接到谷歌服务器的连接将使用这种新算法加密。要查看 Chrome 使用哪种协议打开一个站点，请查看 Chrome 开发工具中的](https://web.archive.org/web/20221208230552/https://www.google.com/chrome/browser/canary.html)[安全面板](https://web.archive.org/web/20221208230552/https://developers.google.com/web/updates/2015/12/security-panel?hl=en)。如果您看到“CECPQ1”，则连接使用了新系统。

有趣的是，我们今天还报道了后量子密码初创公司 PQ 最近筹集的[1030 万美元融资](https://web.archive.org/web/20221208230552/https://beta.techcrunch.com/2016/07/07/quantum-encryption-startup-pq-bags-10-3m-series-a/)。谷歌的消息肯定验证了 PQ 在构建后量子系统方面的工作。