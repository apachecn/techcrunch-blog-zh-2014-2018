# 网络启示录的四骑士 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/01/10/the-four-horsemen-of-the-cyber-apocalypse/>

什洛米·布特纳鲁撰稿人

**编者按:** *Shlomi Boutnaru 是预测网络-安全初创公司 [CyActive](https://web.archive.org/web/20221225130542/http://www.cyactive.com/) 的 CTO 兼联合创始人。*

如果说 2014 年对网络安全有什么好处的话，那就是它向我们展示了大公司、政府和军队是多么容易受到网络攻击。从我们电网的漏洞到我们的收银机，网络攻击已经成为4000 亿美元的问题。虽然和攻击的动机和方法不同，但有四个作案者在全速向我们冲来——我们需要控制他们。

这些“四个 骑士”为我们指出了2015 年我们有望看到黑客使用的组件:无法修补的系统中的漏洞；回收的恶意软件隐藏不易察觉；和人为错误。研究这些先兆可以很好地将我们从潜在的网络灾难中拯救出来。

## 未打补丁和无法打补丁的系统

心脏出血。当你发现你的安全网有漏洞时会发生什么？heart bleed 漏洞是在 Open SSL 中发现的，这是一种数据加密软件，旨在保护敏感信息。当 Heartbleed 在四月份被发现时，它在 IT 界引起了轩然大波，这是因为 OpenSSL 在许多网站的广泛使用以及可以用来对付它的容易获得的漏洞。这些漏洞使得攻击者能够通过软件中的漏洞获取大量敏感信息，如密码和用户名，这些软件本应保护这些信息。

心脏出血具有广泛和长期的影响。虽然和软件的补丁版本已经发布，但是许多被开发来使用 OpenSSL 的和系统并没有更新，因为它们的硬件并不是为更新而构建的。只要这些关键系统还在运行，它们就很容易被利用。

这种危险不是理论上的。2014 年 4 月至 6 月间，450 万名患者的身份证明从社区卫生系统(CHS)医院网络的未更新系统中被盗，该网络在和美国运营着 206 家医院。对网络的初始入侵是通过利用在医院使用的无线网络设备中的【Heartbleed】漏洞实施的，该设备尚未更新。

**Shellshock。**像 Heartbleed 一样，Shellshock 也是一个漏洞，但问题更大，因为它存在于Unix 操作系统的基本命令行中，而不是存在于某些网站使用的软件中。Unix 广泛应用于各种领域，包括路由器和网络服务器(包括 OSX 和 Linux 在内，大约 64%的服务器都是基于 Unix 的)、工业 SCADA 和 747。

和 Heartbleed 一样，Shellshock 震惊了 T21 的 IT 界和网络界，因为它在最广泛使用的操作系统之一的基础上炸开了一个容易被利用的漏洞。既然有补丁可用，Shellshock 造成的主要威胁并不源于它的存在，而是像 Heartbleed 一样，源于许多用 Unix [开发的系统无法在和长期打补丁的事实。](https://web.archive.org/web/20221225130542/http://www.cyactive.com/shellshock-blasts-supermassive-black-hole-heart-cyber-space/)

在许多 Unix 系统中，持续的操作是至关重要的，打补丁需要关闭和机器来重新启动它们。这对我们所有人来说意味着，一个仍在被广泛利用的非常基本的漏洞([9 月份每天有](https://web.archive.org/web/20221225130542/https://twitter.com/eastdakota/status/516457250332741632)150 万次攻击尝试)不会很快消失。从路由器到飞机，Shellshock 将在未来几年内伴随我们的日常生活系统。

## 人为错误和恶意软件重用联手

**黑 PoS。** BlackPoS 暴露了网络安全方面的大规模多层次跨组织失败。组织没有防范已知的恶意软件，人为错误加剧了本已灾难性的局面。

BlackPoS 是一种自 2013 年以来就为人所知的恶意软件，用于从销售点(PoS)系统窃取信用卡信息，它的两个变种在 2014 年的两起重大零售违规事件中被使用。虽然它给零售巨头造成了数亿美元的损失，但黑客可以在网上以 1800 美元的价格购买。在目标零售连锁店发生大规模数据泄露事件后仅四个月，家得宝就被与完全相同的恶意软件的变种攻破，使用与相同的[攻击方法](https://web.archive.org/web/20221225130542/http://www.cyactive.com/go-target-home-depot/)，如果寻找并研究过网络和端点系统中本应注意到的技术。

此外，在这两次攻击中,黑客利用了第三方供应商的安全漏洞，给予他们进入T21 零售商网络和PoS 设备的权限。例如，在目标攻击中，有[证据](https://web.archive.org/web/20221225130542/http://krebsonsecurity.com/2014/01/new-clues-in-the-target-breach/)显示漏洞中首先利用的软件是 BMC 的，是开发IT 管理软件用于目标的公司的。这就是人为错误开始的地方。易于猜测的密码和不受监控的网络连接成为了攻击者的天堂。

这些攻击引发的主要问题是，组织没有彻底研究和关注类似组织被攻破的方式。除了组织本身，网络防御世界需要开发更好的技术来处理已知恶意软件的变种，因为黑客会重复使用和回收它们。

## 当黑客使用廉价的恶意软件来最大化效果时

**蜻蜓。**蜻蜓(又名精力充沛的熊)是一个有能力的攻击者使用廉价、基本和众所周知的恶意工具来对理应受到良好保护的目标产生最佳效果的例子。利用 Java 和 Internet Explorer 中两个广为人知的漏洞利用工具包，加上已知的 SysMain 和 Karagany RAT 恶意软件的变种，蜻蜓的部署者成功获得了对非常敏感目标的访问权限，包括美国和加拿大的航空和国防工业、美国和欧洲的能源电网运营商、主要发电公司、石油管道运营商和工业控制系统(ICS)设备制造商。

虽然这次行动的主要动机似乎是网络间谍活动，但是这些目标中潜在的破坏活动应该给我们敲响警钟。看起来，尽管这些类型的组织在网络防御上投入了数十亿美元，但他们在应对由有能力的攻击者操作的基本威胁时仍有困难。

## 游戏计划

尽管细节仍在浮出水面，索尼最近遭受的攻击表明了人为错误和未被发现的回收恶意软件的危险结合。最初的报告表明，攻击者使用了至少六个[重复使用的](https://web.archive.org/web/20221225130542/http://www.cyactive.com/3-2-1-action-sonys-apocalyptic-scene/)组件，包括两个数据擦除恶意软件，Shamoon 和 Darkseoul，这两个软件都可以在网上免费下载。虽然头条新闻一直被漏洞之前的人为错误所占据，但正确的恶意软件检测形式本可以及时标记这些众所周知的组件，以防止攻击。

虽然索尼只是最新的例子，但 2014 年的网络攻击成为头条新闻，一系列的发现和事件应该会推动我们重塑 T42 的网络防御方式。幸运的是，到目前为止，我们已经避免了一场网络灾难。我不是说天要塌下来了，但是当我们的军队和政府组织、工业联合体和金融机构处于危险之中时，是时候发出警报了，以便推动脆弱的组织(大多数组织都是脆弱的)进一步努力。

因为你不能把你的资源分散到每一个地方，我们把它浓缩成四个骑士，我们认为它们正在制造必须立即解决的危险。研究这些先兆很可能将我们从潜在的网络灾难中拯救出来。

这是对两个组织和网络安全世界的行动呼吁——无法修补的系统和重复使用的恶意软件将成为未来几年中网络攻击的根源，以及下一个潜在的网络灾难。这两个问题都远非简单就能解决，只能通过结合企业和网络专家的知识、资源和增强的意识来解决。

如果我们要成功应对这些未决问题，就需要对所需的主动措施(在补丁、人工智能和其他方面)有一种紧迫感。