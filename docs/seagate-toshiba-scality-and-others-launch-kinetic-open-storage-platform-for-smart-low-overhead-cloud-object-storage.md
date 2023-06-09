# 希捷、东芝、Scality 和其他公司推出 Kinetic 开放式存储平台，用于智能、低开销的云对象存储

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/08/16/seagate-toshiba-scality-and-others-launch-kinetic-open-storage-platform-for-smart-low-overhead-cloud-object-storage/>

# 希捷、东芝、Scality 和其他公司推出 Kinetic 开放式存储平台，用于智能、低开销的云对象存储

两年前，希捷[推出了](https://web.archive.org/web/20230315095316/http://www.theregister.co.uk/2013/10/22/seagate_letting_apps_talk_direct_to_drives/)一种用于硬盘驱动器的[新技术](https://web.archive.org/web/20230315095316/http://www.seagate.com/tech-insights/kinetic-vision-how-seagate-new-developer-tools-meets-the-needs-of-cloud-storage-platforms-master-ti/)，这种技术本质上让应用程序通过以太网连接直接访问[的一些驱动器](https://web.archive.org/web/20230315095316/http://www.seagate.com/products/enterprise-servers-storage/nearline-storage/kinetic-hdd/)，以使用键-值对存储对象。这减少了传统文件系统和文件服务器带来的开销，并允许供应商将更多驱动器装入机架。希捷为 OpenStack 的 Swift 对象存储和 Riak 提供了这项技术的驱动程序，东芝最近也推出了一些基于相同技术的驱动器。

![figure-3-drive-application-software-api-new-612x792](img/25d301c5a5ed86f00ec2e8c8a13415a2.png)现在，一个包括三大硬盘制造商(Seagate、Toshiba 和 Western Digital)以及思科、Cleversafe、戴尔、DigitalSense、NetApp、Open vStorage、Red Hat 和 Scality 的联盟正在加入 Linux 基金会，以开发 Kinect。

Kinect 开放存储项目将作为 Linux 基金会的合作项目来指导开发，目标是“在下一代支持以太网的存储设备上提供开源对象存储”

该项目将以太网连接的规格与驱动器上的密钥/价值存储技术相结合。该项目将管理与这些基于 Kinect 的驱动器接口的 API、开源库和模拟器。

正如 Seagate 在启动这个项目时首次提出的那样，基于文件的老式系统正迅速被基于对象的方法所取代，尤其是在数据中心。

该公司[称](https://web.archive.org/web/20230315095316/http://www.seagate.com/tech-insights/kinetic-vision-how-seagate-new-developer-tools-meets-the-needs-of-cloud-storage-platforms-master-ti/)“新范式是面向对象的:一个图片、电影、电子商务和网络数据、搜索、游戏以及所有这些的档案的世界。这些对象——主要由非结构化数据组成——被写入、读取和删除，但从不被修改，这使它们成为[键/值存储库](https://web.archive.org/web/20230315095316/https://en.wikipedia.org/wiki/Key-value_database)的理想候选对象。

Linux 基金会的执行董事吉姆·泽姆林告诉我，他认为 Kinect 项目是走开源路线的典型案例。这里的合作伙伴显然是竞争对手，但他们希望在硬件上竞争，而不是在软件上竞争——联盟中的软件供应商希望提供管理硬件的工具。

“如果一个项目由一家公司单独领导、拥有和维护，你会在某个时候碰到玻璃天花板，”他指出并补充说，由一家公司编写的软件实在太多了。但是，这些公司需要一个中立的参与者来管理这些项目，并创建一个他们可以聚集和投资这些项目的地方——这就是 Linux 基金会的合作项目的用武之地，这些项目正迅速成为这类开源项目的标准。