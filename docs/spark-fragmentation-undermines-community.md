# 火花分裂破坏社区 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/06/12/spark-fragmentation-undermines-community/>

维诺德·艾扬格撰稿人

Vinod Iyengar 是开源机器学习公司的产品营销总监

[H2O.ai](https://web.archive.org/web/20221208100635/http://h2o.ai/)

.

More posts by this contributor

Hadoop 发行战最终将在 Cloudera 的 CDH 和 Hortonworks 的 HDP 之间展开。情况并非总是如此。

在市场分裂的高峰期，许多公司以这样或那样的形式提供 Hadoop 发行版。这些公司包括亚马逊(Amazon)、Cloudera、Hortonworks、IBM、MapR、Pivotal、Teradata、英特尔和微软(Microsoft)。

竞争是商业的自然组成部分，科技行业也不例外。事实上，正是竞争让最终用户获得了最好的产品。然而，当谈到开源时，情况就有点混乱了。

不像专有产品，它们被期望作为它们自己的小岛运行，开源社区被认为是友好的。那些试图向企业销售开源产品的人提到的优势之一是它们的“即插即用”程度——没有供应商锁定。如果你对一个开源产品的性能不满意，那么撕掉这个产品并用别的东西替换它应该是一个相对无痛的过程。关于 Hadoop 生态系统的争论的问题是，当他们说“Hadoop”时，并不是每个人都指的是同一个东西

Hadoop 不是一个单一的统一产品——它是一个包含一系列模块的框架，比如 HDFS 和 MapReduce。这个术语也可以用来指与 Hadoop 一起工作的其他软件包的更广泛的生态系统，如 Apache Hive、Pig、Spark 等。对于客户来说，这意味着他们对 Hadoop 的看法不像他们想象的那样容易替换。

> 只有一个庞大的、不断增长的、专注的社区才能让 Apache Spark 长期保持相关性。

HDP 和 CDH 不涵盖完全相同的软件包，即使他们这样做，他们也经常不是相同的版本。去年 6 月，木桶公司的 DevOps 工程师德里克·伍德写了一篇[博客](https://web.archive.org/web/20221208100635/http://blog.cask.co/2015/06/hadoop-components-versions-in-distros-matrix/)，展示了 HDP 和 CDH 的哪个版本支持不同软件包的哪个版本。简单地说，要记录的东西很多。在某种程度上，这种“versionitis”背叛了开源，尤其是 Hadoop 所代表的东西。

在过去的一年里，我越来越担心 Apache Spark 生态系统会重蹈 Hadoop 的覆辙。尽管 Apache Spark 只有四年的历史，但我们已经有一些供应商在寻求以不同的形式向客户销售 Apache Spark。

尽管他们有不同的声明，但这些公司通过强迫客户利用他们特定的 Apache Spark 版本和组件，从本质上分裂了 Apache Spark 社区。例如，CDH 5.5.1 支持 Apache Spark 1.5.0，而 HDP 2.3.2.0 支持 Apache Spark 1.4.1。更糟糕的是，现在越来越多的趋势是为特定的发行版构建特性，而这些特性从来不会被提交回上游。

人们可以也应该在开源产品的基础上建立公司(我就为这样的公司工作)。然而，我们对我们的社区和客户有责任确保我们信守开源的承诺。当向客户提供商业发行版时，他们应该尽可能地靠近核心，向上游贡献一切，并支持最新的模块版本。

当建立在学术环境中(加州大学伯克利分校的 AMPLab 在 Apache Spark 的情况下)或供内部使用(想想雅虎的 Hadoop)的开源项目成为大型上市公司或寻求进入公开市场的风险投资公司的领域时，问题不可避免地会出现。开源的理想经常被牺牲在创造一个容易包装的产品的祭坛上，这个产品可以出售以产生短期利润。

但从长远来看，这是不可辩护的。软件正成为一种商品，随着时间的推移，它的生产成本只会越来越低。Apache Spark 本身正受到新的开源技术的攻击，这些技术可能会侵蚀其价值主张。 [Apache Kafka](https://web.archive.org/web/20221208100635/http://kafka.apache.org/) 提供了分析流数据的新方法， [Apache Flink](https://web.archive.org/web/20221208100635/https://flink.apache.org/) 提供了“大数据”的新框架， [Apache Apex](https://web.archive.org/web/20221208100635/https://apex.apache.org/) 统一了流和批处理。

只有一个庞大的、不断增长的、专注的社区才能让 Apache Spark 长期保持相关性。如果工程师发现 Apache 使用起来太麻烦，他们会转向其他东西，因为在供应商创造的割据环境中导航存在固有的困难。受害的将是供应商自己。我们不要让这种情况发生。