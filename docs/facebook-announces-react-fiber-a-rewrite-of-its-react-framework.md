# 脸书宣布推出 React Fiber，这是对其 React 框架的重写

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/04/18/facebook-announces-react-fiber-a-rewrite-of-its-react-framework/>

脸书完全重写了用于构建用户界面的流行 JavaScript 库 [React](https://web.archive.org/web/20230405021555/https://facebook.github.io/react/) 。该公司此前并没有过多谈论这个项目名为 React Fiber 的项目，但实际上它已经在这方面努力了一段时间。现在已经准备好公开谈论这个项目的更多细节(在关于它的消息去年开始传播之后),计划是在今年晚些时候 React 16.0 发布后将这个重写版本交给开发人员。它已经在今天的 Facebook.com 使用，这清楚地表明脸书自己认为它已经准备好了黄金时间。

此外，它还启动了 Relay 的重写，Relay 是构建数据密集型应用程序的框架。

## 反应纤维

该公司告诉我，React Fiber 背后的想法是利用该公司从第一次开发 React 中学到的东西，将其放入一个更新的框架中，该框架仍然完全向后兼容现有的基于 React 的应用程序。脸书告诉我，React Fiber 将成为 React 框架未来任何改进和特性开发的基础。

脸书工程师、React 核心团队成员本·阿尔珀特(Ben Alpert)在本周早些时候的一次采访中告诉我，这里的主要重点是让 React 尽可能响应迅速。“当我们开发 React 时，我们总是在寻找如何帮助开发者更快地构建高质量的应用，”他指出。“我们希望能更容易地开发出性能出色的应用程序，并让它们具有更好的响应能力。”

鉴于这一主题，这个新版本的亮点是用于调度和增量渲染的内置原语就不足为奇了。“我们希望确保在正确的时间呈现正确的内容，”Alpert 说，并补充说“响应能力是一个巨大的推动力。”

但是为什么要从头重写 React 呢？Alpert 说:“旧的代码基础不一定是坏的，但我们希望从一个新的基础开始，它可以为我们未来所做的一切提供动力。”例如，这意味着新代码是从头开始开发的，是可扩展的。

Alpert 强调，React Fiber 将向后兼容，尽管与所有主要的 React 更新一样，将有一些小的突破性变化。不过，该团队表示，预计这对开发者来说不会有问题。“我们一直有一个强大的 API 合同，所以这给了我们重新实现的灵活性，”他补充说。

## 继电器现代

[![](img/aa4da0de34f07a50287df0c10efe413c.png)](https://web.archive.org/web/20230405021555/https://techcrunch.com/wp-content/uploads/2017/04/relay_modern.png) 正如脸书今天所宣布的，Relay——该公司用于构建数据驱动应用的 JavaScript 框架——也被重新编写，同样强调了性能和可扩展性。Relay 结合了 React 和脸书的 GraphQL 查询语言，现在 Relay Modern(该公司称之为“重写”)旨在进一步推动这一概念，并克服原始设计的一些限制。这也意味着简化一些设计来增强框架的整体性能。“Relay Modern 保留了 Relay 的最佳部分——协同定位的数据和视图定义、声明性数据提取——同时还简化了 API，增加了功能，提高了性能，并减小了框架的大小，”该团队在今天的公告中解释道。为了做到这一点，该团队实施了一些更改，但最重要的是，它采用了静态查询和提前优化。

静态查询本质上确保了不会被运行时条件改变的复杂查询可以被预先构建并卸载到脸书的服务器上。因此，应用程序不必通过网络发送复杂的查询，只需发送一个字符串，该字符串标识预先设置的查询以及完成查询所需的变量。与此相关，Relay 编译器中的提前优化功能现在会查看查询结构，以优化现在存储在服务器上的查询，从而更快地执行它，因此也更快地向用户返回结果。例如，React Modern 中的其他新特性包括内置垃圾收集。

对于已经在使用旧版本 Relay 的开发人员来说，Relay Modern 带有一个兼容性 API。

脸书表示，当其团队将脸书应用程序中的市场标签从 Relay 切换到 Relay Modern 时，Android 上的交互时间平均缩短了 900 毫秒。虽然这听起来不多，但移动设备上的每一秒都很重要，这足以让应用程序的响应速度明显比以前更快。