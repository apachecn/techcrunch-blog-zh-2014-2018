# 脸书工具警告开发者警惕钓鱼攻击悬空相似域名 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/05/02/facebook-tool-warns-developers-of-phishing-attacks-dangling-lookalike-domains/>

# 脸书工具警告开发者警惕钓鱼攻击悬空相似域名

网络钓鱼似乎是一个长期存在的问题，所以我张开双臂欢迎任何与之斗争的工具。今天，脸书宣布了一项服务:一项为域名所有者或相关用户提供的服务，该服务可以监视可能预示着网络钓鱼企图的粗略版本的网址。

“开发者只需要指定他们关心的域名，我们的工具会处理剩下的事情，”脸书安全工程师黄大炜解释道例如，如果您订阅了合法域名“facebook.com”的网络钓鱼警报，当我们检测到潜在的网络钓鱼域名(如“facebook.com.evil.com”)和其他恶意域名时，我们会向您发出警报。"

将你的钓鱼网站作为 evil.com 的一个子域似乎是一种赠品。但是还有更微妙的方式来愚弄人们。例如，如果有人想让你认为一封电子邮件来自这个网站，他们可能会注册 techcrunch-support.com 或 techcrunch.official.site 这样的网站，然后从那里发送出去。

拼写上的小变化也起作用:如果你在打电话，走在街上，努力不被骑电动滑板车的人撞到，你会注意到一封来自 techcruhch.com 或 techcrunoh.com 的电子邮件吗？我认为不是。早在一天，甚至 CrouchGear 可能会工作。

内联渲染不同的相似字符是一个奇怪的新威胁:whɑtsɑpp.com 有一个阿尔法(或其他东西)而不是一个 a，并且有益地渲染为 xn—whtspp-cxcc.com。听着，这个系统不是我设计的。我只是用它。

该工具通过观察颁发给新域的证书流，在遇到的域中寻找所有这些变化。“我们一直在使用这些日志来监控为脸书所有的域名颁发的证书，并创建了工具来帮助开发者利用相同的方法，”[在脸书的博客文章](https://web.archive.org/web/20221210034959/https://www.facebook.com/notes/protect-the-graph/phishing-domain-detection/2037453483161459/)中写道。他们真好！

[开发者可以在这里注册](https://web.archive.org/web/20221210034959/http://developers.facebook.com/tools/ct/subscriptions)，提交他们想要监控的域名。脸书不会做任何事情，但提醒你，它检测到一些奇怪的东西，所以如果有一个假阳性，你不必担心被踢出你的领域。另一方面，如果骗子在 doppelgnger 的网址上开店，你就必须亲自跑腿去关闭它，并警告你自己的用户要小心。

[![](img/51f0558f09180477421842cbf4b05f90.png)](https://web.archive.org/web/20221210034959/https://techcrunch.com/tag/f8-2018/)