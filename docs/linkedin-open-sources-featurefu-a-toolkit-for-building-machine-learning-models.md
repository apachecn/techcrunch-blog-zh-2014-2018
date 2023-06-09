# LinkedIn 开源功能 Fu，一个用于构建机器学习模型的工具包 

> 原文：<https://web.archive.org/web/http://techcrunch.com/2015/09/04/linkedin-open-sources-featurefu-a-toolkit-for-building-machine-learning-models/>

# LinkedIn 开源 FeatureFu，一个用于建立机器学习模型的工具包

LinkedIn 今天[宣布](https://web.archive.org/web/20230130225130/https://engineering.linkedin.com/open-source/featurefu-building-featureful-machine-learning-models)开源一个名为 [FeatureFu](https://web.archive.org/web/20230130225130/https://github.com/linkedin/FeatureFu) 的内部工具。FeatureFu toolkit 旨在让开发人员更容易围绕统计建模和决策引擎构建他们的机器学习模型。

这里的想法是利用 LinkedIn 在"[特性工程](https://web.archive.org/web/20230130225130/http://stackoverflow.com/questions/2674430/how-to-engineer-features-for-machine-learning) " 方面的知识，并让公司外部的开发人员也能使用它。在机器学习中，特征工程基本上是利用你对正在观察的现象的详细知识，然后利用这些知识建立机器学习模型。

LinkedIn 认为，大多数大规模推荐系统(想想 LinkedIn 自己在其网站上建议联系的工具)至少由两个团队管理:一个团队处理离线建模，另一个团队负责在线[功能](https://web.archive.org/web/20230130225130/https://en.wikipedia.org/wiki/Feature_(machine_learning))——系统的服务/模型评分部分。这导致了 FeatureFu 试图解决的一系列问题。

“很多大规模的推荐系统是脆弱的，易受攻击的。LinkedIn 高级软件工程师赵兵告诉我:“FeatureFu 允许在这些系统上进行创造性和敏捷的开发，因此发布新功能不需要几周甚至几个月。”。

例如，特征生成方式的微小变化会给另一个团队带来大量的工作，并且也使得实验不同的特征/模型技术变得困难。

FeatureFu 使用一个名为 Expr 的小型 Java 库，开发人员可以用它来转换和构建一组现有的特性。“一旦部署到一个在线特征生成框架，它消除了任何进一步的代码更改的需要，以便为各种各样的派生特征提供模型，”赵描述了该系统的优势。

那么 LinkedIn 为什么决定开源这个工具呢？“当我们对软件有业务需求时，我们首先会查看开源软件中是否有预先存在的软件项目。如果没有，那我们就自己创造，”赵告诉我。“只要软件不是业务区分器，我们就经常开源项目，这样很多人都能受益。”

赵还指出，他希望 FeatureFu 能被广泛采用。“FeatureFu 可能会成为许多机器学习系统的通用技术，”他说。“它使特征工程更加敏捷，这是机器学习应用程序成功的关键之一。所以我们想与业界分享我们的成果。”