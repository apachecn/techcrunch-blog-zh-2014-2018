# 苹果的差分隐私对你的数据和机器学习的未来意味着什么

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/06/14/differential-privacy/>

苹果正在加强其人工智能努力，以与竞争对手保持同步，这些竞争对手一直在机器学习驱动的人工智能高速公路上开足马力，这要归功于他们在挖掘用户数据方面的自由态度。

但苹果并非如此，它将自己标榜为大量渴求数据的公司中唯一的用户隐私捍卫者。当其他数据吸血鬼吞噬位置信息、键盘行为和搜索查询时，苹果却对用户信息嗤之以鼻。该公司不断推出硬件解决方案，使苹果(以及黑客、政府和身份窃贼)更难访问你的数据，并且传统上限制数据分析，因此所有这些都发生在设备上，而不是苹果的服务器上。

但在 iOS 中有几个症结，苹果需要知道用户在做什么，以完善其功能，这对一家将隐私放在第一位的公司来说是一个问题。进入差分隐私的概念，苹果软件工程高级副总裁 Craig Federighi 在昨天的全球开发者大会上简要讨论了这个概念。

“差分隐私是统计学和数据分析领域的一个研究课题，它使用哈希、子采样和噪声注入来实现这种众包学习，同时保持每个个人用户的信息完全隐私，”Federighi 解释道。

差别隐私不是苹果公司的发明；学术界已经研究这个概念很多年了。但随着 iOS 10 的推出，苹果将开始使用差分隐私来收集和分析键盘、聚光灯和笔记中的用户数据。

差分隐私的工作原理是通过算法对个人用户数据进行加扰，使其无法追溯到个人，然后分析大规模数据的大规模趋势模式。目标是保护用户的身份和他们数据的细节，同时仍然提取一些通用信息来推动机器学习。

至关重要的是，iOS 10 会在将你的设备上的数据全部发送给苹果之前，对其进行随机化处理，因此数据永远不会以不安全的形式传输。苹果也不会收集你输入的每一个词或你搜索的每一个关键词——该公司表示，它将限制它可以从任何一个用户那里获取的数据量。

一个不寻常的举动是，苹果公司向宾夕法尼亚大学的 Aaron Roth 教授提供了不同的隐私实施文件，以供同行审查。罗斯是一名计算机科学教授，他写了一本关于差分隐私的书(书名为《差分隐私的算法基础》)，费德里基说，罗斯称苹果在差分隐私方面的工作是“开创性的”。

苹果表示，在推出 iOS 10 之前，它可能会发布更多关于其差异化隐私实施和数据保留政策的细节。

那么这对你意味着什么呢？

## 键盘

苹果昨天在 WWDC 的主题演讲中宣布了对 iMessage 的重大改进。差分隐私是这些改进的关键组成部分，因为苹果公司希望收集数据，并用它来改善 QuickType 和 emoji 的键盘建议。在 iOS 9 中，QuickType 会学习短语并更新你个人设备上的词典——因此，如果你键入“thot”或“on fleek”的次数足够多，“自动更正”最终会停止将短语改为“Thor”和“on fleet”

但在 iOS 10 中，苹果将使用差分隐私来识别其数十亿用户的语言趋势——所以你会在使用键盘之前就获得键盘建议新俚语的神奇体验。

“当然，让软件更加智能的一个重要工具是发现多个用户如何使用他们的设备的模式，”Federighi 解释道。“例如，你可能想知道哪些新单词是流行的，这样你就可以在 QuickType 键盘上更容易地提供它们。”

不同的隐私也将彻底解决关于哪些表情符号最受欢迎的争论，允许你的表情符号键盘重新排序，这样就不会不方便地把心藏在最后面，靠近随机的十二生肖和鸢尾花。

## 聚光灯

差分隐私建立在 iOS 9 中引入的[深度链接的基础上，以改进 Spotlight 搜索。费德里吉在去年的 WWDC 上用菜谱的例子揭示了深度链接。他演示了在 Spotlight 中搜索“土豆”可以从安装在他设备上的其他应用程序中找到食谱，而不仅仅是显示网页结果。](https://web.archive.org/web/20230331183418/https://techcrunch.com/2015/06/08/apple-lets-you-search-within-apps-with-a-deep-link-search-api-in-ios-9/)

随着越来越多的信息被储存在应用程序中，超出了传统搜索引擎的范围，深度链接是使内容可搜索的必要条件。然而，[关于 iOS 9 将如何对深度链接搜索结果进行排名，以防止应用开发者用不相关的建议淹没聚光灯的问题](https://web.archive.org/web/20230331183418/https://medium.com/ios-os-x-development/deep-linking-search-in-ios-9-will-change-everything-feab0bb7e189#.gmn166s73)仍然存在。

苹果计划使用差别隐私来解决这一问题。通过模糊的用户数据，苹果可以识别出非常受欢迎的深层链接，并为它们分配更高的排名——因此，当你使用 Spotlight 寻找土豆食谱时，你会得到像 Yummly 这样的应用程序提供的最美味的土豆准备的建议。

## 笔记

Notes 是 iOS 10 将应用通过差分隐私收集的信息来改进功能的最后一个领域。

Federighi 还在昨天的主题演讲中讨论了 Notes 的升级。在 iOS 10 中，笔记将变得更具互动性，为可操作的信息加下划线——因此，如果你在笔记中记下朋友的生日，它可能会在日期下加下划线，并建议你创建一个日历事件来记住它。

为了做出这种聪明的建议，苹果再次需要知道哪种笔记在其广大用户中最受欢迎，这需要不同的隐私。

## 它是如何工作的

那么到底什么是差分隐私呢？宾夕法尼亚州立大学计算机科学与工程系副教授亚当·史密斯说，这不是一项单一的技术，他和罗斯一起参与这一领域的研究已经有十多年了。

相反，它是一种数据处理方法，内置限制以防止数据与特定个人相关联。它允许对数据进行整体分析，但会在从单个设备上获取的数据中注入噪声，因此在批量处理数据时，个人隐私不会受到影响。

“从技术上讲，这是一个数学定义。它只是限制了你处理数据的方式。它以这样一种方式限制他们，使他们不能在数据集中链接太多关于任何单个区间拾取点的信息，”Smith 说。

他将差分隐私比作能够在一台调谐不良的收音机上，从一层静电噪音中挑出一段潜在的旋律。“一旦你明白你在听什么，就很容易忽略静电干扰。所以，任何一个个体都有点像这样——你对任何一个个体都了解不多，但总的来说，你可以看到相当清晰的模式。

“但是，如果你不通过添加这种噪声来约束自己，它们就不会像你得到的那样清晰和准确。史密斯告诉 TechCrunch:“这就是你为人们的隐私提供更强有力的保障所付出的代价。

Smith 认为苹果是第一家试图大规模利用差分隐私的大公司，尽管他指出其他大型商业实体如美国电话电报公司之前已经对此进行了研究(也许令人惊讶的是，[谷歌通过其项目 Rappor](https://web.archive.org/web/20230331183418/https://github.com/google/rappor) 也进行了研究)。他指出，初创公司也对此感兴趣。

尽管没有其他商业实体像苹果现在打算的那样大规模部署差分隐私，但史密斯补充说，这个概念的鲁棒性是毋庸置疑的，尽管他指出，它确实需要正确实施。

“与任何与安全相关的技术一样，细节是魔鬼。它必须得到很好的实施。但对于这个基本想法的合理性，没有争议。”

## AI 的未来？

史密斯说，苹果对差分隐私的采用对该领域来说非常令人兴奋，这表明它可能会导致机器学习技术如何运作的巨大变化。

硅谷关于隐私的辩论通常是从执法的角度来看待的，将用户隐私与国家安全对立起来。但对科技公司来说，争论的焦点是用户隐私与功能。苹果引入差别隐私可能会从根本上改变这场争论。

谷歌和脸书等公司一直在努力解决如何提供功能丰富且私密的产品的问题。谷歌的[新消息应用 Allo](https://web.archive.org/web/20230331183418/https://techcrunch.com/2016/05/19/google-engineer-says-hell-push-for-default-end-to-end-encryption-in-allo/) 和脸书的 Messenger 都没有默认提供端到端加密，因为两家公司都需要对用户的对话进行真空处理，以改善机器学习并允许聊天机器人运行。苹果也想从用户数据中收集见解，但它不愿意为了这样做而放弃 iMessage 的端到端加密。

史密斯表示，苹果选择实施差异隐私将使公司对保护隐私和改善机器学习之间的权衡进行不同的思考。“我们不需要收集那么多，”史密斯说。“这些类型的技术是考虑隐私的一种真正不同的方式。”

尽管 iOS 10 只会使用差分隐私来改进键盘、深度链接和笔记，但史密斯指出，如果证明成功，苹果可能会在地图、语音识别和其他功能中使用该策略。史密斯建议，苹果还可以寻找人们使用某些应用程序的时间之间的相关性。

苹果选择不收集原始用户数据，这可能会增加用户的信任。方便的是，这也有助于苹果加强自身对抗政府入侵的能力——众所周知，这是苹果在与联邦调查局的法庭斗争中争取的目标。

由于差分隐私已经研究了十年，对苹果来说这是一个相对低风险的安全策略。史密斯说，苹果采用这一概念，在创新和用户安全之间找到了“最佳平衡点”。

“不管他们是否完全成功，我认为这将完全改变对话，”史密斯说。“我认为，人们对收集私人信息的看法将因此发生巨大变化。这可能最终会成为这个项目给苹果公司留下的最大遗产，可能远远超出苹果公司自身的财务影响。”