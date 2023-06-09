# 流程即代码:勇敢新世界的安全运营协调 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/03/06/process-as-code-security-ops-orchestration-for-a-brave-new-world/>

桑迪普·巴德拉撰稿人

Sandeep Bhadra 是

[Menlo Ventures](https://web.archive.org/web/20221208201121/https://www.menlovc.com/)

专门投资网络安全创业公司。

网络犯罪是一个巨大的问题——联邦政府、美国最大的公司和数千万个人的克星。但是现在有合理的希望，很大一部分网络犯罪问题最终可以得到解决。

尽管最高级别的攻击非常复杂，但超过 90%的[攻击都是在地下市场购买现成组件的基础上构建的低级攻击。](https://web.archive.org/web/20221208201121/http://www.secureworks.com/assets/pdf-store/white-papers/wp-underground-hacking-report.pdf)

这是一个好消息——击退这些普通的攻击要比高度复杂、资金充足的攻击容易得多。但该行业还面临着其他挑战。

典型的安全运营中心(SOC)缺乏训练有素的安全专家来监控公司数字足迹的健康和安全。安全研究人员需要近十年的时间来获得防御现代攻击的技能。弗罗斯特和沙利文预测，到 2020 年，训练有素的安全专家将短缺 150 万人。SOC 团队在处理大量低影响事件时不堪重负，未能及时做出响应，或者完全错过了标记严重攻击的早期事件警报。

似乎有一个解决方案来处理这一巨大的人力短缺和授权足球队。人们正在努力将过程记录为代码，或者简单地说，使用软件来自动化重复但耗时的任务，同时提高单个安全专家的生产力。

其中大部分是所谓的 [SecOps](https://web.archive.org/web/20221208201121/http://www.fiercedevops.com/story/what-secops-and-why-should-you-care/2015-08-20) orchestration。

一些历史背景很重要。SecOps 是一个更加成熟的 DevOps 运动的模拟，它围绕着一个简单的想法发展，即把常见的 IT 过程记录为代码，并在 IT 团队之间进行协作。

这使得新的、有用的功能可以在几天内开发、测试并投入生产，而不是几周。如今，像 [Puppet](https://web.archive.org/web/20221208201121/https://puppetlabs.com/) 、 [Docker](https://web.archive.org/web/20221208201121/https://www.docker.com/) 、 [HashiCorp](https://web.archive.org/web/20221208201121/https://www.consul.io/) 、 [Ansible](https://web.archive.org/web/20221208201121/https://www.ansible.com/) (一家最近被红帽收购的 Menlo 投资组合公司)和 [Atlassian](https://web.archive.org/web/20221208201121/https://www.atlassian.com/software/jira) 这样的公司开发的 DevOps 工具使 IT 团队能够以每小时多次的频率推出新功能和变化！

SecOps orchestration 本质上采用 DevOps 方法，并将其应用于安全领域，以更好地调查和响应事件。它端到端地管理安全事件的生命周期，作为一个一致的业务流程，用代码以“剧本”或“处方”的形式记录下来

SecOps 的潜力远远大于今天的事故响应。如今，响应安全事件是一个将不同工具拼凑在一起的手动过程，这些工具包括日志记录系统、网络流量分析器、第三方威胁情报馈送、数据取证和软件修补、备份和恢复。使用这种方法，识别根本原因并修复攻击的影响可能需要几周或几个月的时间。

> 如今，私人安全专家正独自手动对抗他们的对手。

相比之下，拥有大量在线基础设施足迹的先驱，如网飞和谷歌，已经在借鉴 SecOps 剧本，用代码自动化日常任务。其中包括重新映像终端、跟踪电子邮件网络钓鱼攻击、协调网络和终端设备之间的数据以及更新防火墙权限，所有这些都提高了处理安全事件的速度。

我相信一个成功的 SecOps 编排平台可以通过专注于少数业务和架构优先事项为自己开拓一个大型独立业务——基于开放 API 的自动化，一个共享最佳实践和直观 UI 的中立社区。

为了有效地实现自动化，来自 [Phantom](https://web.archive.org/web/20221208201121/https://www.phantom.us/) 、 [CyberSponse](https://web.archive.org/web/20221208201121/https://cybersponse.com/) 和 [Invotas](https://web.archive.org/web/20221208201121/https://www.fireeye.com/products/security-orchestrator.html) (最近被 FireEye 收购)的 SecOps 编排平台依赖于从第三方供应商构建的各种安全设备中读取和写入的“配方”。如今，像银行这样的大客户——他们计划每年花费 15 亿美元用于网络安全——正迫使供应商开放他们的 API，并与其他供应商友好合作。软件/云设备和健壮的开放 API 作为它们的公共接口的出现，使得构建编排产品变得更加容易。

公司还必须学会团结起来，建立和分享这些自动化配方。毕竟，对付在黑帽市场上购买的恶意软件的一个好方法是建立一个白帽市场或好人社区！

美国国防部已经有了这样的举措，但是私人安全专家和供应商现在对共享数据持怀疑态度，部分原因是他们在多国管辖范围内运营。像 [FIDO](https://web.archive.org/web/20221208201121/https://github.com/Netflix/Fido) (一个由网飞团队发起的开源项目)和 Phantom 的[社区剧本库](https://web.archive.org/web/20221208201121/https://github.com/phantomcyber/playbooks)这样的厂商中立的开放框架创造了一个良性循环，吸引了安全专家来构建他们自己的剧本和最佳实践编码方案。

最后，出色的工作流、用户界面和设计是构建跨 IT 团队的无缝编排和协作的关键。 [Resilient Systems](https://web.archive.org/web/20221208201121/https://www.resilientsystems.com/) 和 FireEye/Invotas 已经构建了出色的工作流工具，帮助 SecOps 团队以一致的方式响应事件。[德米斯图拉](https://web.archive.org/web/20221208201121/https://dbot.demisto.com/)有一个现代化的协作方法，通过 Slack 的消息用户界面构建一个安全编排机器人。

这一领域的初创公司正在努力解决一个普遍存在的大规模问题，并实现最佳网络安全实践的民主化。而且他们倾向于与供应商无关，这使他们能够很好地构建反映客户最佳利益的社区和产品。

如今，私人安全专家正独自手动对抗他们的对手。明天，他们将团结起来，在代码中实现最佳实践，并最终建立一个针对坏人的高效防御。