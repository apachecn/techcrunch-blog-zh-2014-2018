# DigitalOcean 与 CoreOS 合作，将大规模集群部署引入其平台

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/09/05/digitalocean-partners-with-coreos-to-bring-large-scale-cluster-deployments-to-its-platform/>

# DigitalOcean 与 CoreOS 合作，将大规模集群部署引入其平台

自从几年前推出以来， [DigitalOcean](https://web.archive.org/web/20230405201950/http://digitalocean.com/) 迅速成为一个价格合理的虚拟服务器托管平台。然而，该公司的野心远远超出了在 5 美元/月的机器上托管你的 WordPress 博客或测试服务器，今天它在这个方向上迈出了下一步，宣布支持 [CoreOS](https://web.archive.org/web/20230405201950/https://coreos.com/) ，这是一个非常受欢迎的以容器为中心的 Linux 发行版，用于大规模部署。

DigitalOcean 的联合创始人兼 CMO 米奇·怀纳(Mitch Wainer)在今天的一份声明中表示:“CoreOS 的社区非常兴奋。“我们很高兴地宣布，随着开发人员大规模扩展能力的提高，他们可以立即开始使用 CoreOS，确保其架构的弹性。”

DigitalOcean 告诉我，它相信它的平台现在是“在任何云服务上试用 CoreOS 和开始使用容器的最简单和最便宜的方式”

鉴于运行 CoreOS 集群比在一台服务器上运行最新版本的 Ubuntu 要复杂得多，DigitalOcean 用户还需要采取一些额外的步骤。当他们创建一个新的服务时，需要提供一个[配置文件](https://web.archive.org/web/20230405201950/https://coreos.com/docs/cluster-management/setup/cloudinit-cloud-config/)(或者用 DigitalOcean 的说法是“droplet”)。毕竟，CoreOS 需要知道它可以与哪些其他服务器对话。设置这些配置文件并不复杂，但也绝不简单。

随着 CoreOS 支持的加入，DigitalOcean 显然试图将其触角延伸到基本虚拟服务器市场之外。如果它想在与 AWS 和谷歌云平台的竞争中受到重视，它确实需要提供这类服务。

正如该公司的联合创始人 Ben Uretsky】经常告诉我的，该公司在过去几年中忙于扩大规模以满足需求，以至于像添加更多发行版这样的基本产品开发经常被搁置。现在，DigitalOcean 有了充足的资金和更多的员工，它可以更加专注于增加新功能，比如今天的 CoreOS 发布。