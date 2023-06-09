# 谁在进行常识性推理，为什么这很重要 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2014/08/09/guide-to-common-sense-reasoning-whos-doing-it-and-why-it-matters/>

凯瑟琳·哈瓦西撰稿人

**编者按:** *[Catherine Havasi](https://web.archive.org/web/20221129023842/http://web.media.mit.edu/~havasi/) 是剑桥一家基于人工智能的文本分析公司 [Luminoso](https://web.archive.org/web/20221129023842/http://www.luminoso.com/) 的首席执行官兼联合创始人。Luminoso 建立在麻省理工学院媒体实验室近十年的研究基础上，研究如何将自然语言处理和机器学习应用于文本分析。凯瑟琳还领导着“开放思维常识项目”，这是世界上最大的常识知识库之一，是她在 1999 年与马文·明斯基和普什·辛格共同创立的。*

想象一下，你从墨西哥度假回来后，在街上遇到一个朋友。

“你的假期过得怎么样？”你的朋友问。

“真是太棒了。我们对这次旅行非常满意，”你回答。"天气不太潮湿，尽管水有点冷。"

没什么好惊讶的，对吧？你和你的朋友都知道你用“湿度”来指天气，用“寒冷”来指海洋

现在想象一下，你试着和一台电脑进行同样的对话。你的回答可能会是类似于“是的。不是。计算。”

部分问题在于，当我们人类交流时，我们依赖于大量未言明的假设背景。每个人都知道“水是湿的”，而且“人们想要快乐”，我们假设我们遇到的每个人都分享这一知识。它构成了我们如何互动的基础，让我们能够快速、高效、有深度地交流。

尽管今天的技术很先进，但当它成为社会日常生活的一大部分时，它的主要缺点是它不同意这些假设。

我们发现自己越来越多地对着我们的设备说话——对着我们的手机，甚至是我们的电视。但当我们与 Siri 交谈时，我们经常发现，如果我们远离简单的命令，她背后的规则就无法准确理解我们想要的东西。为了实现这一愿景，我们需要计算机理解我们，就像我们在自然环境中相互交谈一样。为此，我们需要继续发展常识推理领域——没有常识推理，我们永远无法与 Siri、谷歌眼镜或我们的 Xbox 进行智能对话。

## 什么是常识推理？

常识推理是人工智能的一个领域，旨在通过找到收集这些假设并教给计算机的方法，帮助计算机更自然地理解人并与人互动。常识推理在自然语言处理领域最为成功，尽管在其他领域也有值得注意的工作。这个机器学习领域，有着奇怪的名字，正开始悄悄渗透到不同的应用中，从文本理解到处理和理解照片中的内容。

如果没有常识，在一个日益数字化和移动化的世界中，很难构建适应性强和无人监管的 NLP 系统。当我们互相交谈和在线交谈时，我们尽可能地变得有趣，并利用新的方式来表达事情。重要的是创造能与我们并驾齐驱的计算机。

事情远比人们想象的要复杂。如果我问你一只长颈鹿是否适合你的办公室，你可以很容易地回答这个问题，尽管事实上你很可能从来没有想象过一只长颈鹿住在你的办公室里，在你最喜欢的 Pandora 电台播放背景音乐时，静静地在你的榕树上咀嚼。这是一个完美的例子，说明你不仅了解这个世界，而且知道如何将你的世界知识应用到你以前没有想过的事情上。

常识系统的强大之处在于它们具有高度的适应性，能够适应各种各样的主题，如餐馆评论、徒步旅行鞋调查和临床试验，而且速度快、准确度高。这是因为我们从使用新单词的上下文中理解它们。我们利用常识猜测词义，然后提炼这些猜测，我们已经建立了一个类似的系统。此外，当我们理解复杂或抽象的概念时，我们有可能通过对简单概念进行类比来做到这一点，这是乔治·莱考夫在他的书《我们赖以生存的隐喻》中描述的理论。简单的概念是常识。

常识推理有两大思想流派。一方使用更像逻辑或基于规则的表示，而另一方使用更多基于联想和类比的推理或“基于语言的”常识——后者得出的结论更模糊，但更接近自然语言的工作方式。

不管你是否意识到，你每天都在和这两种系统打交道。

你可能听说过 IBM 的 [Watson](https://web.archive.org/web/20221129023842/http://en.wikipedia.org/wiki/Watson_(computer)) ，它在 Jeopardy 中赢得了著名的胜利，但一个不太为人知的事实是，Watson 的前身是一个名为 [Cyc](https://web.archive.org/web/20221129023842/http://en.wikipedia.org/wiki/Cyc) 的项目，它是由 Doug Lenat 在 1984 年开发的。Cyc 的开发者被称为 [Cycorp](https://web.archive.org/web/20221129023842/http://www.crunchbase.com/organization/cycorp) ，运营着一个基于逻辑的常识事实的大型知识库。它今天仍然活跃，并且仍然是最大的基于逻辑的常识项目之一。

在基于语言的常识学校，马文·明斯基、普什·辛格和我于 1999 年启动了“开放思维常识”项目。OMCS 和它更著名的分支 ConceptNet 包括一个纯文本的信息库，以及一个大的知识图表。该项目在众包方面取得了早期成功，现在 ConceptNet 包含了 1700 万种语言的事实。

## **为什么现在很重要？**

在过去的几年里，特定类型的机器学习取得了长足的进步:[基于向量的机器学习](https://web.archive.org/web/20221129023842/http://en.wikipedia.org/wiki/Support_vector_machine)和[深度学习](https://web.archive.org/web/20221129023842/http://en.wikipedia.org/wiki/Deep_learning)。他们在推进基于语言的常识方面发挥了重要作用，从而使计算机更接近人类处理语言的方式。

NLP 是常识推理的优势所在，这项技术正开始进入商业产品。虽然还有很长的路要走，但常识推理将在未来几年继续快速发展，这项技术足够稳定，可以在今天投入商业使用。它比现有的本体和基于规则的系统，或者简单地基于机器学习的系统具有显著的优势。

用不了多久，你就可以和你的电脑就你的墨西哥之旅进行更常识性的对话了。当你告诉它水有点冷时，你的电脑会回答:“很抱歉听到海洋很冷，每年的这个时候都是这样。不过我看了你旅行的照片，看起来你得穿上上周买的那件可爱的新泳衣。”