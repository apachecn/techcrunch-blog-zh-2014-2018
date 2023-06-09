# 微软研究院展示了“DeLorean”，这是一项构建无延迟云游戏服务的技术 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/08/22/microsoft-research-shows-off-delorean-its-tech-for-building-a-lag-free-cloud-gaming-service/>

# 微软研究院展示了“DeLorean”，这是一项建立无延迟云游戏服务的技术

![delorean](img/fa121fc2ece778ed5844f36cf7dfc84b.png)

展望游戏的未来，很少有概念像神话中的“游戏网飞”那样让人兴奋这是一个我们已经以多种形式看到的概念，从 [OnLive 的](https://web.archive.org/web/20221208010123/https://games.onlive.com/)早期努力到[索尼新的 PlayStation Now 服务。](https://web.archive.org/web/20221208010123/https://beta.techcrunch.com/2014/08/02/sony-and-ea-experiment-with-new-business-models-for-older-games/)

与在你自己的主机或个人电脑上运行游戏的传统模式相比，从庞大的服务器集群中提供游戏有几个优势。它允许任何可以播放流媒体视频的设备玩高清游戏；图形可以以稳定的速度提高，因为云架构的改进比新的控制台硬件更容易推出；游戏可以立即玩，而不是等待大约 20GB 的游戏下载。

虽然微软在发布自己的流媒体游戏平台方面没有索尼走得那么远，但它之前就对这个概念表现出了兴趣。就在今年 4 月，微软展示了像《泰坦陨落》这样的大预算 Xbox 大片的开发者如何利用 Azure 云平台来包括更好的人工智能和物理，而不降低整体性能。

昨天,[微软研究院发布了一份报告](https://web.archive.org/web/20221208010123/http://research.microsoft.com/apps/pubs/default.aspx?id=226843),表明该公司正在寻找方法，在未来某个时候利用其云计算专业知识创建一个独特的云游戏平台。它讨论了 DeLorean，这是一个“投机的执行引擎”，尽管微软的 Azure 服务器和玩家的设备之间存在无数网络延迟，但它使从云中交付看似无延迟的游戏成为可能。

该报告得出结论，参与研究的大多数用户无法区分在本地系统上玩[毁灭战士 3](https://web.archive.org/web/20221208010123/http://bethsoft.com/en-us/games/doom_3_bfg) 和[寓言 3](https://web.archive.org/web/20221208010123/http://www.lionhead.com/games/fable-iii/) 这两个相对动作繁重的游戏，还是从使用 DeLorean 的云上玩，延迟为 250 毫秒。这是一个游戏改变者——大多数经历这种滞后的游戏玩家会沮丧地扔掉他们的控制器。

微软研究院是如何实现这一壮举的？DeLorean 的关键是“投机”描述符。视频游戏通常不能像 YouTube 或网飞的视频一样被缓冲，因为玩家的动作会影响屏幕上发生的事情——如果我在《泰坦陨落》中开枪，游戏显示我在跳跃，我会很生气。但是，通过查看以前的玩家输入，并对*最有可能的*玩家动作进行采样，微软找到了一种方法来预测你可能会采取的几个动作，并提前发送每个动作的视频，让它在游戏进行过程中向玩家显示最准确的猜测。

这种解决方案的最大问题是它的带宽非常大:微软指出，其预测引擎的比特率比简单地发送游戏根据实际玩家输入知道准确的帧高 1.5-4.5 倍。这意味着你需要更快的连接才能通过理论上的 Xbox 流媒体服务玩游戏，而不是 PlayStation Now 或 Nvidia 的 Grid，但你不会体验到游戏玩家不靠近托管这些服务的物理服务器时出现的口吃。