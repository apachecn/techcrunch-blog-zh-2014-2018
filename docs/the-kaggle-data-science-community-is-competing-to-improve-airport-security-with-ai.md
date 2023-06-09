# Kaggle 数据科学界正在与 AI TechCrunch 竞争提高机场安全性

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/06/22/the-kaggle-data-science-community-is-competing-to-improve-airport-security-with-ai/>

# Kaggle 数据科学界正在竞相利用人工智能改善机场安全

通过机场安检是一个普遍的痛苦经历。尽管速度缓慢且具有侵犯性，但美国运输安全管理局在捕捉威胁方面并没有很好的记录。在 [Kaggle](https://web.archive.org/web/20221117173045/https://www.kaggle.com/) 数据科学社区的帮助下，国土安全部(DHS)正在举办一场在线竞赛，以构建机器学习驱动的工具，这些工具可以增强代理，理想情况下使整个系统同时更加准确和高效。

今年早些时候被谷歌收购的[ka ggle](https://web.archive.org/web/20221117173045/https://beta.techcrunch.com/2017/03/07/google-is-acquiring-data-science-community-kaggle/)定期举办在线比赛，数据科学家通过开发复杂机器学习问题的新方法来争夺资金。[今天提高威胁识别算法的比赛](https://web.archive.org/web/20221117173045/https://www.kaggle.com/c/passenger-screening-algorithm-challenge#description)将是 Kaggle 今年的第三次发布，奖金超过 100 万美元。

最高奖金为 50 万美元，奖金总额为 150 万美元，参赛者必须准确预测身体上威胁物体的位置。美国运输安全管理局正在向竞争对手提供其图像数据集，以便他们可以根据携带武器的人的图像进行训练。重要的是，这些将是由 TSA 创建的舞台图像，而不是真实世界的例子——这是确保隐私的必要举措。

计算机视觉初创公司 Matroid 的创始人兼首席执行官礼萨·扎德告诉我:“比赛的结果将是一个很好的指标，表明我们可以期待这样的系统工作得多好。”。“至少，我们应该有这样一个系统来增强现有的安全警卫，以确保他们不会错过危险的物品。”

当然，TSA 面临的问题不仅仅是机器学习问题。昂贵的物理机升级起来很复杂，而且没有一台具备现代数据中心的复杂 GPU。值得庆幸的是，谷歌、脸书和其他公司正在边缘(没有互联网)大量投资机器学习框架的轻量级版本，优化为在本地运行。

这意味着这次比赛的一些参赛作品可能会在实际的扫描机器上使用——这只是一个事先训练和优化约束条件的问题。DHS 承诺将与获奖者密切合作，探索潜在的现实世界应用。

“这是一个非常困难的问题，机器没有疯狂的 GPU，”Kaggle 的创造者安东尼·戈德布卢姆(Anthony Goldbloom)在一次采访中告诉我。"但是有一点被忽略了，那就是做推理不一定需要如此繁重的计算."

Kaggle 和 TSA 必须考虑的另一个问题是影响自动威胁检测流程的偏见风险——这可能是旅行者的一个潜在噩梦，可能会根据任意因素进行不适当的隔离。为了缓解这种情况，TSA 投入了特别的精力来创建图像数据集，最终将用于训练探测器。

“美国运输安全管理局在这方面做得很好，”戈德布卢姆强调说。“他们招募志愿者，但确保他们有足够的多样性，这样模型就不会在某一类型的人身上失败。”

谷歌计划在不久的将来向竞争对手开放 GCP。尽管谷歌拥有 Kaggle，但谢天谢地它没有强迫人们使用它自己的开源框架 TensorFlow。您可以点击查看更多详情[；比赛将于 12 月结束。](https://web.archive.org/web/20221117173045/https://www.kaggle.com/c/passenger-screening-algorithm-challenge#description)