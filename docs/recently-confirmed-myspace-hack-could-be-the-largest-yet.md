# 最近证实的 Myspace 黑客攻击可能是迄今为止最大的 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/05/31/recently-confirmed-myspace-hack-could-be-the-largest-yet/>

你可能多年都没有想到过——更不用说访问过——Myspace。(对，还在附近。今年早些时候，时代公司收购了 Viant，从而获得了 it 和其他资产。)但不幸的是，用户数据永远不会真正消亡。对于 Myspace 的新主人来说，这是一个坏消息，因为该公司[在美国阵亡将士纪念日假期周末之前证实](https://web.archive.org/web/20221205195632/http://www.businesswire.com/news/home/20160531005770/en/Time-Confirms-Breach-Myspace)，它已经收到警报，大量被盗的 Myspace 用户名和密码组合在一个在线黑客论坛上出售。

然而，这些数据是好几年前的了。在 2013 年 6 月 11 日之前，它似乎仅限于旧 Myspace 平台整体用户群的一部分，当时该网站重新推出，增加了安全性。

时代公司没有证实有多少用户账户包含在这个数据集中，但是来自 LeakedSource.com[的一份报告称，涉及超过 3.6 亿个账户。每条记录都包含一个电子邮件地址、一个密码，在某些情况下，还有第二个密码。由于一些账户有多个密码，这意味着总共有超过 4.27 亿个密码可供出售。](https://web.archive.org/web/20221205195632/https://www.leakedsource.com/blog/myspace)

尽管这一数据泄露事件可以追溯到几年前，但有问题的数据集的规模使其引人注目。Sophos [的安全研究人员表示](https://web.archive.org/web/20221205195632/https://nakedsecurity.sophos.com/2016/05/31/myspace-breach-could-be-the-biggest-ever-half-a-billion-passwords/)这可能是有史以来最大的数据泄露事件，轻松超过[最近因 2012 年的一次黑客攻击而在网上曝光的 1.17 亿封 LinkedIn 电子邮件和密码](https://web.archive.org/web/20221205195632/https://nakedsecurity.sophos.com/2016/05/31/myspace-breach-could-be-the-biggest-ever-half-a-billion-passwords/)。

这一估计似乎站得住脚—[虽然还有许多其他大规模的数据泄露事件，但即使是一些最大的事件也没有这种规模。](https://web.archive.org/web/20221205195632/http://www.informationisbeautiful.net/visualizations/worlds-biggest-data-breaches-hacks/)美国选民数据库泄露包括 1.91 亿条记录，Anthem 为 8000 万条，易贝为 1.45 亿条，Target 为 7000 万条，Experian 为 2 亿条，Heartland 为 1.3 亿条，等等。

这些旧数据泄露的问题是，它们来自一个安全措施没有今天这么强的时代。这意味着这些密码很容易被破解。LeakedSource 指出，这些被破解的前 50 个密码占了 600 多万个密码，占总数的 1.5%，给你一个规模感。

密码以无盐 SHA-1 散列的形式存储，LinkedIn 也是如此。

这使得时代公司在一定程度上确定了数据泄露的日期，因为该网站在 2013 年 6 月重新启动，加强了账户安全，包括存储密码的双盐哈希。它还证实，这次违规对其任何其他系统、用户信息或其他媒体财产没有影响，泄露的数据也不包括任何财务信息。

Myspace 正在通知用户，并已经取消了已知受影响帐户的密码。

该公司还使用自动化工具，试图识别和阻止任何可能发生在 Myspace 账户上的可疑活动。

Myspace 的首席财务官杰夫·拜尔斯托在一份声明中说:“我们非常重视客户数据和信息的安全和隐私——尤其是在这个恶意黑客越来越老练，各行各业的违规行为变得司空见惯的时代。”。“我们的信息安全和隐私团队正在尽一切努力支持 Myspace 团队。”

然而，虽然黑客本身和产生的数据集可能是旧的，但仍然可能有影响。因为如此多的在线用户只是在多个网站上重复使用他们的相同密码，所以能够将给定用户名或电子邮件与密码相关联的黑客可以在其他网站上破解用户的当前帐户。

当然，用户甚至不太可能记得他们几年前在 Myspace 上使用的密码，这使得保护你当前的账户更加困难。更好的选择是始终使用更复杂的密码，定期重置密码，并利用密码管理工具(如 Dashlane 或 LastPass)来帮助您跟踪您的登录。

Myspace 也证实了这次黑客攻击是由化名为“和平”的俄罗斯黑客所为这也是对 [LinkedIn](https://web.archive.org/web/20221205195632/https://beta.techcrunch.com/2016/05/18/117-million-linkedin-emails-and-passwords-from-a-2012-hack-just-got-posted-online/) 和 [Tumblr](https://web.archive.org/web/20221205195632/https://staff.tumblr.com/post/144263069415/we-recently-learned-that-a-third-party-had) 攻击负责的同一个人。在 Tumblr 的案例中，大约有 6500 多万个账户受到影响。但是这些密码被“加盐”，这意味着它们更难破解。

Myspace 表示，由于此案仍在调查中，该公司正在与执法部门合作。