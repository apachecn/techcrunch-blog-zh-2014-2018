# 谷歌从运行 Kubernetes 开发基础设施 TechCrunch 后退了一步

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/08/29/google-steps-back-from-running-the-kubernetes-infrastructure/>

Google today [宣布](https://web.archive.org/web/20230109104857/https://cloud.google.com/blog/products/gcp/google-cloud-grants-9m-in-credits-for-the-operation-of-the-kubernetes-project)将向[云计算原生计算基金会](https://web.archive.org/web/20230109104857/https://www.cncf.io/) (CNCF)提供 900 万美元的 Google Cloud 信用额度，以帮助[进一步推进其在 Kubernetes container orchestrator 上的工作](https://web.archive.org/web/20230109104857/https://www.cncf.io/announcement/2018/08/29/cncf-receives-9-million-cloud-credit-grant-from-google)，并且将该项目的运营控制权移交给社区。这些额度将在三年内分摊，用于支付构建、测试和分发 Kubernetes 软件的基础设施成本。

为什么这很重要？到目前为止，谷歌托管了几乎所有支持该项目的云资源，如其 CI/CD 测试基础设施、容器下载和云上的 DNS 服务。但是谷歌现在后退了一步。随着 Kubernetes 社区达到成熟状态，Google 正在将所有这些转移到社区中。

在测试基础设施和托管容器下载之间，Kubernetes 项目定期在 5，000 台虚拟机上运行超过 150，000 个容器，因此运行这些系统的成本迅速增加。自项目启动以来，Kubernetes 容器注册表已经提供了近 1.3 亿次下载。

另外值得注意的是，CNCF 现在包括了很多通常会相互竞争的成员。例如，我们正在谈论阿里云、AWS、微软 Azure、谷歌云、IBM 云、甲骨文、SAP 和 VMware。所有这些都得益于 CNCF 和 Kubernetes 社区的工作。谷歌没有直截了当地这么说，但可以合理地假设，它也希望其他人承担一些运营 Kubernetes 基础设施的负担。同样，社区的一些成员肯定也不希望与谷歌的基础设施如此紧密地联系在一起。

谷歌 Kubernetes 引擎产品经理 William Deniss 在今天的公告中写道:“通过与项目的贡献者分担 Kubernetes 的运营责任，我们期待看到所有 Kubernetes 贡献者为项目运营带来的新想法和效率。”。他还指出，许多谷歌公司仍将参与运营 Kubernetes 基础设施。

“谷歌对 Kubernetes 社区的重大财政捐赠将有助于确保该项目不断创新和广泛采用的步伐不会减弱，”CNCF 的执行董事丹·科恩说。“我们很高兴看到 Google Cloud 将 Kubernetes 测试和基础设施项目的管理转移到贡献者手中——使该项目不仅是开源的，而且是由开放社区公开管理的。"

目前还不清楚该项目是否计划将一些谷歌托管的基础设施转移到另一个云上，但它肯定会这样做——其他云提供商也可以提供类似的信用。