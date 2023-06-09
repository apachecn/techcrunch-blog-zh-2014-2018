# OpenAI 的机器人手不需要人类来教它人类行为

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/07/30/openais-robotic-hand-doesnt-need-humans-to-teach-it-human-behaviors/>

用手抓东西是你在婴儿时期学会的第一件事，但这远不是一件简单的事情，随着你的成长，它只会变得更加复杂和多变。这种复杂性使得机器很难教会自己做什么，但 Elon Musk 和 Sam Altman 支持的 OpenAI 的研究人员创造了一个系统，它不仅像人类一样持有和操纵物体，而且完全自主地发展了这些行为。

许多机器人和机器人手已经精通某些抓握或运动——工厂中的机器人可以比人更灵巧地挥动枪栓。但是，让机器人如此出色地完成任务的软件很可能是手写的，并且非常特定于应用程序。例如，你不能给它一支铅笔，让它写字。即使是同一生产线上的某些东西，比如焊接，也需要全新的系统。

然而对于一个人来说，拿起一个苹果和拿起一个杯子并没有太大的不同。存在差异，但我们的大脑会自动填补空白，我们可以即兴创作新的抓握方式，安全地握住不熟悉的物体等等。这是机器人严重落后于人类模型的一个领域。此外，你不能只训练一个机器人做人类做的事情——你必须提供数百万个例子来充分展示人类会用成千上万个给定的对象做什么。

OpenAI 的研究人员认为，解决方案是根本不使用人类数据。相反，他们让计算机在模拟中一次又一次地尝试和失败，慢慢地学习如何移动手指，以便它抓住的物体按照预期移动。

这个被他们称为 Dactyl 的系统只被提供了手指的位置和手中物体的三个摄像头视图——但请记住，当它被训练时，所有这些数据都是模拟的，发生在虚拟环境中。在那里，计算机不必实时工作——它可以在几秒钟内尝试一千种不同的抓取物体的方式，分析结果，并将数据反馈给下一次尝试。(手本身是一只[影子灵巧手](https://web.archive.org/web/20230316000453/https://www.shadowrobot.com/products/dexterous-hand/)，也比大多数机器人手复杂。)

除了系统需要学习的不同对象和姿势，还有其他随机参数，如指尖的摩擦量，场景的颜色和照明等等。你还不能模拟现实的每一个方面，但是你可以确保你的系统不仅仅在蓝色的房间里，在有特殊标记的立方体上工作。

他们在这个问题上投入了大量的力量:6144 个 CPU 和 8 个 GPU，“在 50 个小时内收集了大约一百年的经验。”然后，他们第一次将该系统应用到现实世界中——它展示了一些令人惊讶的类似人类的行为。

我们用手做的事情，甚至没有注意到，比如转一个苹果来检查是否有瘀伤，或者给朋友递一杯咖啡，使用许多小技巧来稳定或移动物体。Dactyl 重新创造了其中的几个，例如用拇指和单指握住物体，同时用其他手指旋转到所需的方向。

这个系统的伟大之处不仅仅在于其运动的自然性，以及它们是通过反复试验独立实现的，还在于它不依赖于任何特定形状或类型的物体。就像人类一样，Dactyl 可以抓住和操纵你放在它手里的任何东西，当然是在合理的范围内。

这种灵活性被称为一般化，对于必须与现实世界互动的机器人来说，这很重要。不可能为世界上的每个对象和情况手工编码单独的行为，但一个机器人可以适应并填补空白，同时依靠一套核心理解，可以混过去。

与 OpenAI 的其他工作一样，[描述结果的论文可以免费获得](https://web.archive.org/web/20230316000453/https://d4mucfpksywv.cloudfront.net/research-covers/learning-dexterity/learning-dexterity-paper.pdf)，正如他们用来创建和测试 Dactyl 的一些工具一样。