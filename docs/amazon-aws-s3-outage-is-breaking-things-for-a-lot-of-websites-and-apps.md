# 亚马逊自动气象站 S3 站的中断对许多网站和应用程序来说是一个突破

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/02/28/amazon-aws-s3-outage-is-breaking-things-for-a-lot-of-websites-and-apps/>

亚马逊的 S3 网络存储服务正在经历广泛的问题，导致其依赖的网站、应用和设备的服务部分或全部中断。AWS 产品为许多网站提供图像托管，也托管整个网站和应用后端，包括 Nest。

根据[亚马逊的 AWS 服务健康仪表板](https://web.archive.org/web/20230324132154/https://status.aws.amazon.com/)的说法，S3 的中断是由于“美国东部-1 S3 的高错误率”，该公司还表示正在努力“补救这个问题”，但最初没有透露任何进一步的细节。

受影响的网站和服务包括 Quora、时事通讯提供商 Sailthru、Business Insider、Giphy、许多出版商网站的图像托管、Slack 中的文件共享等等。联网灯泡、恒温器和其他物联网硬件也受到影响，由于停电，许多人无法控制这些设备。

根据 [SimilarTech](https://web.archive.org/web/20230324132154/https://www.similartech.com/technologies/amazon-s3) 跟踪的数据，亚马逊 S3 被大约 148，213 个网站和 121，761 个唯一域使用，它作为内容主机的受欢迎程度特别集中在美国。它被前 100 万个网站中的 0.8%使用，这实际上比 CloudFlare 小得多，后者被全球前 100 万个网站中的 6.2%使用——但它仍然有这么大的影响。

令人惊讶的是，即使是 AWS 服务状态页面上的状态指示器也依赖于 S3 来存储其健康标记图形，因此尽管有明显的相反证据，该网站仍然显示所有服务为绿色。

我们正密切关注这一情况，一旦有消息，我们将提供更多信息。

**更新(太平洋时间上午 11:40):**AWS 至少修复了自己仪表板的问题——现在[将准确反映服务状态，因为它将继续尝试修复问题](https://web.archive.org/web/20230324132154/https://twitter.com/awscloud/status/836662601090134017)。

**更新(太平洋时间上午 11:57):**AWS 表示，他们相信他们已经“理解了 S3 问题的根本原因”，并且正在“努力修复”它没有透露这一原因的细节。

**更新(PT:12:15PM):**网络智能软件提供商[虽然](https://web.archive.org/web/20230324132154/https://igysrybwz.share.thousandeyes.com/view/tests/?roundId=1488310800&metric=loss&scenarioId=pathVisualization&testId=337583&serverId=105778)指出当前问题的所有数据包丢失似乎都发生在弗吉尼亚州阿什伯恩地区。亚马逊在阿什伯恩有一个 AWS 数据中心，由于其建设过程中发生火灾，其确切位置在去年的一则新闻中被披露。

**更新(12:54 PM PT):** AWS 表示，它看到了“S3 对象检索、列表和删除的恢复”，这意味着您可能会看到头像和其他视觉资源在某些地方出现。该公司还表示，预计在接下来的一个小时内，错误率将进一步改善。

**更新(1:20 PM PT):** 根据 AWS 状态页面，S3 在现有对象的检索、列表和删除方面现已完全恢复，并且正在努力恢复正常运行，以便向位于 S3 的存储中添加新项。

**更新(PT 2:10PM):**AWS 表示，就解决所看到的错误率而言，它现在已完全恢复，S3 服务现在“正常运行”。