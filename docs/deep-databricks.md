# Databricks 发布了 Apache Spark 的无服务器平台以及支持深度学习的新库 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/06/06/deep-databricks/>

# Databricks 发布了 Apache Spark 的无服务器平台以及支持深度学习的新库

今天，为了启动 Spark Summit，Databricks 宣布了 Apache Spark 的无服务器平台，这对希望减少集群管理时间的开发人员来说是个好消息。简化开发人员体验的举措将成为整个活动的主题。除了无服务器之外，该公司还引入了深度学习管道，这是一个很容易将深度学习框架与 Spark 相结合的库。

如果您没有关注过基于云的数据处理的最新发展，Databricks 是开源 Apache Spark 项目的商业表现。该公司的工程师每天都在开发工具来支持 Spark 生态系统，就像今天宣布的那些一样。

随着数据在大型企业决策中的比重越来越大，新用户面临着处理数据管道和云基础设施的巨大挑战。与您可能想的相反，无服务器并不意味着没有服务器也能进行数据操作。这仅仅意味着用户可以通过从一个受管理的计算资源池中获取资源来完成任务，从而减少了每个用户进行低级修补的需要。

“SQL 是无状态的，所以使用它并不难，但是让数据科学无服务器很难，因为它有状态，”Databricks 首席执行官 Ali Ghodsi 在一次采访中向我解释道。

如果说无服务器是 Databricks 在广度上的尝试，那么深度学习管道则是该公司在深度上的尝试。我仍然不会说 TensorFlow 和其他比较深入的学习框架“容易”使用，但是它们比 LISP 更容易使用。这使得深度学习成为越来越多的工作流的一部分，尽管它的使用还不太常见。

“如果你想分配张量流，你必须手动构建图形，并把什么东西引导到什么机器上，”古尔西补充道。“如果你想在 100 台机器上运行，那真的很难。”

Databricks 新的开源库使开发人员能够将深度学习模型转换成 SQL 函数。用户可以使用 Spark MLlib Pipelines 进行迁移学习，并通过 Spark 获得分布式计算的优势。

最后，Ghodsi 指出，Databricks 的结构化流现已普遍可用。该应用编程接口支持顺序数据流的处理。该公司表示，在结构化流开发过程中，它优先考虑最大限度地减少延迟。对于处理异常检测等问题的客户来说，这最终会带来成本和速度两方面的影响。