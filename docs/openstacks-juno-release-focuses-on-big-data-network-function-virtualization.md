# OpenStack 的 Juno 版本专注于大数据、网络功能虚拟化 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/10/16/openstacks-juno-release-focuses-on-big-data-network-function-virtualization/>

[OpenStack](https://web.archive.org/web/20221207203851/http://www.openstack.org/) ，这款用于构建公共云和私有云的开源软件得到了众多[行业巨头](https://web.archive.org/web/20221207203851/http://www.openstack.org/foundation/companies/)的支持，今天发布了 [Juno](https://web.archive.org/web/20221207203851/https://wiki.openstack.org/wiki/ReleaseNotes/Juno) ，这是其最新的单点版本。

像往常一样，这一版本包括对该平台所有服务的更新，这些服务现在涵盖了从云计算到存储服务、身份管理和处理大量数据的工具的所有领域。然而，今天发布的亮点是增加了一个新的数据处理服务，该服务可以自动提供大数据集群，增加了对对象存储的更细粒度的策略控制，以及对[网络功能虚拟化](https://web.archive.org/web/20221207203851/http://en.wikipedia.org/wiki/Network_Functions_Virtualization) (NFV)的初始支持，这是 OpenStack 在电信行业的用户一直要求的。

正如 OpenStack 基金会的首席运营官·马克·科利尔本周早些时候告诉我的那样，这个版本清楚地显示了 OpenStack 用户和运营商的指纹。这方面最好的例子可能是 NFV。“我相信这对 OpenStack 来说是一个非常大的机会，”Collier 告诉我。有了 NFV，电信公司以及运营自己网络的大型企业可以将许多网络服务从昂贵的专有硬件转移到商用服务器上。这带来了巨大的潜在成本节约，但软件栈也必须非常稳定，并提供实时性能。

“如果我是一家电信公司，想要将语音通话的硬件系统转移到软件系统，”科利尔指出，“我需要知道这个活力层不会开始掉线。”在这个初始版本中，团队主要关注性能，并将在未来的版本中继续提供更多的功能。

OpenStack Juno 版本的主要新功能是推出该平台的新数据处理服务。这可以自动调配和管理 Hadoop 和 Spark 集群以进行大数据分析。该服务最初是一个简单的 Apache Hadoop 服务，但随着时间的推移，开发人员也增加了对 HortonWorks 和 Cloudera 的 Hadoop 以及 Spark 的支持。

在我们的采访中，Collier 还指出，他认为 OpenStack 的对象存储增加了更细粒度的策略，这对许多用户来说是一个重要的更新。这样，用户可以更好地控制他们希望如何跨后端和区域存储、复制和访问数据。例如，通常您有可以轻松复制的数据，因此您不需要在任何时候都有三个备份。

通过此次更新，OpenStack 还推出了跨 OpenStack 云的联合身份验证。例如，像 CERN 这样的 OpenStack 用户拥有自己的私有云，然后在公共服务上增加容量。现在，他们可以给研究人员一套凭证，让他们访问这两个。

总的来说，Juno 版本提供了 310 项新功能和 3，200 个错误修复。你可以在这里找到更详细的发行说明[。](https://web.archive.org/web/20221207203851/https://wiki.openstack.org/wiki/ReleaseNotes/Juno)