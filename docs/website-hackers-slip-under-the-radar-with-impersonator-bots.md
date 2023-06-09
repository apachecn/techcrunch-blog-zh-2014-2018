# 网站黑客通过模仿机器人躲过了雷达

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/03/14/website-hackers-slip-under-the-radar-with-impersonator-bots/>

**编者按:** *Ofer Gayer 是 [Incapsula](https://web.archive.org/web/20230228035718/http://www.incapsula.com/) 的安全研究员。*

去年 12 月底，一家金融服务提供商联系了我们，他开始注意到在线注册请求激增。这种激增不是由年终销售工作导致的，而是由有针对性的垃圾邮件攻击引起的，这些攻击使组织充斥着虚假的注册表单，其中大多数表单看起来很有信誉，不会一看到就丢弃。

担心的原因是，该公司出于内部原因，需要对每个新的注册表单进行手动背景检查，然后才将其移交给销售部门。因此，当这个小型背景调查团队在看似合法的在线表格的洪流中开始崩溃时，所有的在线销售业务都停止了。在快速检查该公司的网站流量后，很快就发现客户实际上遇到的是恶意的 bot 活动。

在这种情况下，bot 操作员对组织有足够的了解，可以将手动背景调查过程识别为“软肋”，这可以用来撬动公司的整个销售漏斗。

为了利用这一弱点，犯罪者手工制作了一个垃圾邮件机器人，其唯一目的是用不符合任何容易识别的模式的细节来攻击特定的注册表。最令人担忧的是，这些机器人将自己伪装成普通的人类用户，拥有类似浏览器的 HTTP 指纹和一些功能，使他们能够绕过网站基于挑战的访问控制机制。

这不是我们第一次遇到如此复杂的机器人，它们专门用来模仿人类行为，并在类似浏览器的身份掩护下运行。总的来说，我们喜欢称它们为“模仿机器人”这种自动化工具专为秘密行动而设计，因其能够绕过常见的安全措施而受到青睐，不仅被黑客用于垃圾邮件攻击，还被用于窃取数据、劫持服务器和执行 DDoS 攻击以及其他邪恶活动。

## 这些模仿机器人是谁？

许多类型的不良机器人在互联网上漫游，从垃圾邮件发送者和垃圾邮件发送者到更复杂的漏洞扫描器和 DDoS 机器人。如果其他坏机器人可以比作执行指挥官命令的训练有素的士兵，那么模仿机器人就是特种作战部队。这些“突击队”执行相同的恶意活动，但他们这样做是秘密的，通常使用更先进的攻击技术。

通常，它们基于现有的恶意软件工具，经过修改后可以创建类似浏览器的 HTTP 指纹。这使他们能够绕过阻止较低级/通用版本的安全挑战。模仿者机器人会对公司网站和网络应用程序造成重大损害，导致停机、经济损失和声誉受损。

在 2013 年和 2014 年之间，我们看到[的整体 bot 流量从所有 web 访问的 61.5%下降到 56%，扭转了前两年观察到的上升趋势。然而，尽管总流量下降，模仿机器人的数量继续增长。](https://web.archive.org/web/20230228035718/https://www.incapsula.com/blog/bot-traffic-report-2014.html)

事实上，在过去的三年里，模仿者是唯一一种持续增长的坏机器人，这对大多数网站所有者来说不是好兆头。

网络安全经常被描述为军备竞赛，这是有充分理由的。黑客和白帽子一直试图领先对方一步。当一方找到更好的防守方法时，另一方通常会发展出更聪明的进攻方式。模仿机器人是这种升级的副产品——它们是黑客对网站所有者越来越多地使用反机器人解决方案的回应。

## 模仿机器人是黑客的首选工具

模拟机器人的一种使用方式是漏洞扫描和自动黑客攻击。这种“黑客机器人”是专有工具和脚本，用于系统地扫描网站漏洞，并随意大量利用它们。漏洞一经发布，寻找未打补丁系统的寻宝游戏就开始了。

在 2014 年 9 月发现 [Shellshock 超级漏洞](https://web.archive.org/web/20230228035718/https://techcrunch.com/gallery/what-you-need-to-know-about-shellshock/)之后，我们看到了这种动态的一个很好的例子。

在 Shellshock 发现并发布补丁后不久，我们[看到](https://web.archive.org/web/20230228035718/https://www.incapsula.com/blog/shellshock-bash-vulnerability-28-days-after.html)扫描器流量爆炸。其中一些是担忧的互联网公民的合法扫描尝试。然而，超过 90%的机器人是恶意扫描器和其他恶意自动工具(如 DDoS 恶意软件)，用于探测 Shellshock 漏洞。

对于黑客来说，发起这样的漏洞扫描运动只是“办公室里的另一天”在 2014 年的其他重大漏洞之后，我们已经看到了同样的动态，例如 Heartbleed，以及 Slider Revolution 和 FancyBox 等流行的 WordPress 插件中的漏洞。

这种模仿者僵尸程序还包括来自匿名代理的 DDoS 僵尸程序，这只是攻击者掩盖其真实身份的另一种方式。这是模仿机器人使用的相同 MO。事实上，在过去几个月中，我们已经看到使用 TOR 和其他公开可用的匿名代理来执行应用层 DDoS 攻击(例如 HTTP floods)的僵尸程序显著增加。创建这些代理是为了实现匿名网页浏览——用一个无法追踪的代理代替用户的 IP 地址。

使用匿名代理(大多数是免费的)对 DDoS 攻击者有很多好处。这使他们能够掩盖他们的机器人 IP，让他们绕过基于黑名单的安全解决方案。匿名代理不是为每个 bot 请求使用一个地址，而是在多个 IP 之间传播请求，允许它们在速率限制机制的雷达下飞行。

除了隐藏 IP 之外，匿名代理还会混淆报头信息，使它们能够规避仅基于 HTTP 指纹的安全措施。利用这些固有的好处，犯罪者能够以最小的努力创造一个大的僵尸网络风格的影响。

随着恶意机器人的发展和变得更加隐蔽，知道访问者是谁已经不够了(例如，通过签名阻止)。安全解决方案首先还需要评估为什么会有任何 bot。使用信誉和行为分析可以帮助检查 bot 访问的上下文，这是识别模仿者、匿名代理和其他新型 bot 威胁的重要因素。

## 展望未来

机器人是互联网生态系统的重要组成部分。然而，它们现在不仅仅是工具；它们是用于好的还是恶意的目的，完全取决于拥有者的意图和动机。

当谈到网络威胁时，坏的机器人是当今网络罪犯的首选工具；我们的研究人员发现，超过 90%的所有网络攻击(例如 DDoS 攻击、web 应用程序威胁)都是由他们执行的，而冒充者机器人是坏机器人的精英突击队。

就收入损失和补救工作而言，此类攻击的成本很容易达到数十万甚至数百万美元。正如我们在索尼黑客攻击等重大数据泄露事件中看到的那样，最糟糕的情况实际上取决于攻击者的意图和目标的大小。