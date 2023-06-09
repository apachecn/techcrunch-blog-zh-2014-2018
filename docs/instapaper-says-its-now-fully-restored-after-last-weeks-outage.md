# Instapaper 表示，在上周的中断后，现在已经完全恢复了

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/02/14/instapaper-says-its-now-fully-restored-after-last-weeks-outage/>

Instapaper [今天表示](https://web.archive.org/web/20221005200557/http://blog.instapaper.com/post/157227609796)它已经从长时间的停电中完全恢复，上周停电导致服务中断一天多，然后恢复了有限的容量。广受欢迎的书签服务[在被 Pinterest 收购时拥有数百万用户，上周](https://web.archive.org/web/20221005200557/https://beta.techcrunch.com/2017/02/10/instapaper-goes-down-for-over-a-day-says-a-full-restore-will-take-a-week/)因其 AWS 托管数据库达到系统极限而遭遇中断。

当公司[在 2 月 9 日发布](https://web.archive.org/web/20221005200557/http://blog.instapaper.com/post/157045376396)关于服务中断的消息时，服务已经中断了 31 个小时。为了更快地恢复在线，Instapaper 决定只将用户最近六周保存的文章恢复在线。这允许人们继续标记和阅读他们最近的保存，但不包括该服务的大得多的档案。

当时，Instapaper 表示，它认为恢复其档案可能还需要一周时间，并承诺最迟将在 2 月 17 日星期五之前让它们全部上线。

该公司在给用户的一封电子邮件中表示，太平洋时间今天凌晨 1 点，Instapaper 完全恢复了服务。

电子邮件解释说:“我们在不丢失任何旧文章、对更新文章的更改或从中断中恢复后保存的文章的情况下进行了恢复。”

该公司还在电子邮件中详细介绍了宕机本身，并且[在 Medium 上发布了 Pinterest 产品工程师 Brian Donohue 撰写的完整事后分析](https://web.archive.org/web/20221005200557/https://medium.com/making-instapaper/instapaper-outage-cause-recovery-3c32a7e9cc5f#.z62d2b3il)。在这里，他解释说根本原因是 2014 年 4 月之前创建的 RDS 实例的 2 TB 文件大小限制导致的数据故障。Instapaper 存储用户保存文章的“书签”表在上周的周三达到了极限，导致了错误。

Donohue 说，该团队对数据库的限制一无所知，也没有任何东西可以提醒他们这一事实。

“据我们所知，RDS 控制台中没有监控、警报或日志记录形式的信息可以让我们知道我们正在接近 2TB 文件大小限制，或者我们首先会受到它的限制。即使是现在，也没有任何迹象表明我们的托管数据库存在严重问题，”他写道。

Instapaper 对 Pinterest 网站可靠性工程团队和亚马逊关系数据库服务团队表示感谢，他们在周末与团队合作，加快了恢复过程，使他们提前完成了任务。

尽管如此，该公司坚持认为，问题本身“既难以预测也难以预防，而且中断的性质极其罕见，不太可能再次发生，”Instapaper 给用户的电子邮件指出。

这一声明应该会平息一些用户的担心，即自从被 Pinterest 收购后，书签产品就没有得到工程资源和关注。

此外，该团队还从大修中吸取了宝贵的教训。这让该公司意识到，它没有针对这种情况的灾难恢复计划，它将在未来解决这一问题。Instapaper 目前正在开发一个系统，该系统将立即向 Pinterest 的网站可靠性工程团队升级问题，并将每月测试其 MySQL 备份，而不是每三个月一次，该公司表示。