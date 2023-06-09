# Abbyy 在服务器故障 TechCrunch 中泄露了 203，000 份敏感客户文档

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/08/27/abbyy-leaked-203000-sensitive-customer-documents-in-server-lapse/>

光学字符识别软件制造商 Abbyy 在一个数据库服务器没有密码的情况下保持在线后，暴露了一批敏感的客户文档。

被暴露的服务器是由前 Kromtech 安全研究员[鲍勃·迪亚琴科](https://web.archive.org/web/20221208195434/https://twitter.com/MayhemDayOne)发现的，他现在独立工作。在[发表前分享的一篇博文](https://web.archive.org/web/20221208195434/https://www.linkedin.com/pulse/abbyy-exposed-its-document-storage-database-more-than-bob-diachenko)中，他说公司的一台 MongoDB 服务器被错误地配置为公共访问。他告诉 TechCrunch，服务器[包含 203，896 份扫描文件](https://web.archive.org/web/20221208195434/https://www.linkedin.com/pulse/abbyy-exposed-its-document-storage-database-more-than-bob-diachenko)，包括自 2012 年以来的合同、保密协议、备忘录和其他高度敏感文件。

这些数据还包括企业用户名和加密密码。

总部位于莫斯科的公司[专门从事文档捕获](https://web.archive.org/web/20221208195434/https://techcrunch.com/2017/06/22/abbyys-new-version-of-textgrabber-is-a-super-useful-ocr-and-translation-app/)产品和服务，包括将物理文档转换为跨一系列语言的可搜索和可索引的数字内容。

该公司声称为数千家组织和超过 5000 万用户提供服务。

在本月早些时候的一次私人披露后，该服务器被下线。Abbyy 在周一的一封电子邮件中证实了这一曝光，但没有说明为什么存储服务器对任何人开放。

发言人 Anna Ivanova-Galitsina 说:“该事件涉及一个而不是几个客户和载有商业信息的文件。”"已经及时通知了客户，我们正在合作采取纠正措施."

“(迪亚琴科)一通知我们，我们就锁定了对文件的外部访问。我们已经发出了所有法律要求的通知，并对我们的基础设施、流程和程序进行了全面的纠正性安全审查，”该发言人说。该公司表示，此次曝光是“一次性事件，不会危及公司的任何其他服务、产品或客户”，但指出“进一步的分析正在进行中。”

记者发稿时，该公司不愿证实受影响客户的姓名。Abbyy 拥有数十家主要的全球客户，包括大众汽车、百事可乐、麦当劳和澳大利亚税务局。

Abbyy 没有说是否还有其他人访问了数据库。

这是迪亚琴科最近几个月发现的一系列曝光的 MongoDB 数据库中最新的一个[,包括拥有 3100 万用户的](https://web.archive.org/web/20221208195434/https://www.bleepingcomputer.com/news/security/mongodb-server-exposes-babysitting-apps-database/)[流行虚拟键盘应用](https://web.archive.org/web/20221208195434/https://www.zdnet.com/article/popular-virtual-keyboard-leaks-31-million-user-data/)和最近[用于连接保姆的应用](https://web.archive.org/web/20221208195434/https://www.bleepingcomputer.com/news/security/mongodb-server-exposes-babysitting-apps-database/)。

MongoDB 因其可伸缩性和多功能性而在企业中广泛使用，但是今天仍在使用的许多旧版本的数据库软件在默认情况下没有密码。去年，黑客通过下载和删除服务器上的内容，利用了数千个暴露的服务器——实际上是用它们来勒索赎金。