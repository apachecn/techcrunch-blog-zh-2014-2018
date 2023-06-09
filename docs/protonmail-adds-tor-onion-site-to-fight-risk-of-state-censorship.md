# 质子化邮件增加 Tor onion 网站以对抗国家审查的风险技术危机

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/01/19/protonmail-adds-tor-onion-site-to-fight-risk-of-state-censorship/>

总部位于瑞士的 PGP 端到端加密电子邮件提供商[质子化邮件](https://web.archive.org/web/20221209073354/https://beta.techcrunch.com/tag/protonmail/)现在有了一个洋葱地址，允许用户通过直接连接到 Tor 匿名网络来访问其服务——该公司称这是一项旨在抵御国家发起的审查的积极措施。

这家初创公司迄今为止已经为其 e2e 加密电子邮件服务积累了 200 多万用户，一年多前刚刚推出测试版的[表示，它担心亲隐私工具在州一级被屏蔽的风险增加——这指向了最近的举措，比如加密消息应用](https://web.archive.org/web/20221209073354/https://beta.techcrunch.com/2016/03/17/protonmails-encrypted-email-service-exits-beta-adds-ios-android-apps/) [Signal 在埃及被屏蔽](https://web.archive.org/web/20221209073354/https://beta.techcrunch.com/2016/12/26/1431709/)，以及[英国通过了扩张性的监控立法](https://web.archive.org/web/20221209073354/https://beta.techcrunch.com/2016/11/29/yes-the-uk-now-has-a-law-to-log-web-users-browsing-behavior-hack-devices-and-limit-encryption/)[强制要求跟踪网络活动](https://web.archive.org/web/20221209073354/https://beta.techcrunch.com/2015/11/04/cementing-uk-surveillance-state/)，还可以要求公司避开 e2e 加密和[后门产品](https://web.archive.org/web/20221209073354/https://beta.techcrunch.com/2016/07/15/uk-surveillance-bill-includes-powers-to-limit-end-to-end-encryption/)

去年秋天唐纳德·特朗普(Donald Trump)当选美国总统后，该服务的注册数量也有所增加——鉴于即将上任的总司令的广泛数字监控能力，网络用户显然在寻找一家非美国的安全电子邮件提供商。

“鉴于质子邮件最近的增长，我们意识到在某些国家对质子邮件的审查是不可避免的，我们正在积极努力防止这种情况发生，”创始人安迪·延在发布会上的声明中说。Tor 提供了一种绕过某些互联网块的方法，所以提高我们与 Tor 的兼容性是自然的第一步。"

Tor 浏览器的用户现在可以通过其新的洋葱地址:
[https://质子泵抑制剂 xow.onion](https://web.archive.org/web/20221209073354/https://protonirockerxow.onion/)

这里还有关于如何在 Tor [上设置 ProtonMail 的书面说明。](https://web.archive.org/web/20221209073354/https://protonmail.com/support/knowledge-base/tor-setup/)

通过 Tor 访问 ProtonMail 的用户将使他们的连接匿名——这意味着电子邮件服务将无法看到(因此无法被迫泄露)他们的真实 IP 地址。

当然，仍然可以通过 Tor 浏览到 ProtonMail 的主网站，但它指出直接洋葱地址有一些优势——例如在 Tor 级别上提供 e2e 加密；这意味着 Tor 应用的加密一直存在，直到连接到达 ProtonMail 的基础设施(相比之下，非 onion Tor 连接在最后一个节点之外没有 Tor 加密)，从而使攻击者很难对用户的连接进行中间人攻击。

洋葱网站还提供端到端的认证，ProtonMail 表示，这有助于缓解互联网上广泛使用的现有认证机构(CA)系统的一些[弱点——指出许多 CA 在默认情况下是可信的，有些 CA 可以直接受政府控制。出于这个原因，它也只使用 HTTPS 的洋葱网站——也作为备份以防 Tor 本身被入侵。](https://web.archive.org/web/20221209073354/https://zeltser.com/how-digital-certificates-are-used-and-misused/)

“如果有一天 Tor 遭到破坏，强制执行 HTTPS 将为最终用户增加一层安全保护。同样，Tor 还提供安全保护，以防 HTTPS 受到威胁。它在一篇关于发布的博客中写道:“T4 HTTPS 受到威胁的说法是我们非常重视的，考虑到有数百个 ca 被默认信任，其中许多处于高风险国家的政府直接控制之下。”。

“因此，通过使用我们的洋葱网站，您的电子邮件受到三层端到端加密的保护，外层是 Tor 的加密，中间层是 HTTPS，PGP 是电子邮件本身的最后一道防线。”

它提出推出 Tor hidden 服务的另一个激励因素是加强其对 DDoS 攻击的防御——鉴于攻击者更难确定 onion 网站的物理位置和 IP 地址，因此它可以在持续 DDoS 攻击使其网址离线的情况下提供访问 ProtonMail 的变通办法。

ProtonMail 在 2015 年 11 月遭遇了重大事故，电子邮件服务中断超过 24 小时。Yen 告诉 TechCrunch，它仍然“经常”受到重大的 DDoS 攻击，尽管他认为它的防御和网络现在能够“在不影响用户的情况下”抵御这些攻击。

“也就是说，Tor 对标准 DDoS 攻击的抵抗是我们感兴趣的事情，特别是因为 DDoS 攻击的规模在过去一年中持续增长，”他补充道，尽管他强调这仍然是“与我们对认证机构系统和政府授权阻止的妥协的担忧相比的次要动机”。

ProtonMail 的洋葱网站在这一点上被描述为“实验性的”，所以它的警告可靠性“可能没有我们的标准网站高”——甚至超过了用户通常获得的通常较慢的连接。

“即使不使用 Tor，您的 ProtonMail 收件箱仍然受到 [PGP 端到端加密](https://web.archive.org/web/20221209073354/https://protonmail.com/security-details)、[安全认证](https://web.archive.org/web/20221209073354/https://protonmail.com/blog/encrypted_email_authentication/) (SRP)和可选的[双因素认证](https://web.archive.org/web/20221209073354/https://protonmail.com/support/knowledge-base/two-factor-authentication/)的强力保护。然而， ProtonMail 肯定有用户处于敏感情况下，Tor 提供的额外安全性和匿名性确实可以挽救生命，”它补充道。