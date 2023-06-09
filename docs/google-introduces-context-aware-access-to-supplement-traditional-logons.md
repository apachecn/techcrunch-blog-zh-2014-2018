# 谷歌推出“情境感知”身份识别来补充传统登录技术

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/07/25/google-introduces-context-aware-access-to-supplement-traditional-logons/>

# 谷歌引入“情境感知”识别来补充传统登录

我们现在知道，用户名和密码是保护应用程序和在线服务的一种糟糕的方式，但它们在很大程度上仍然是安全武器库中的一个关键工具。麻烦的是，随着近年来所有的安全漏洞从 [Equifax](https://web.archive.org/web/20230117204849/https://techcrunch.com/2017/09/07/equifax-data-leak-could-involve-143-million-consumers/) 到 [Anthem](https://web.archive.org/web/20230117204849/https://techcrunch.com/2015/02/04/health-insurance-provider-anthem-reports-massive-data-breach/) 到 [Target](https://web.archive.org/web/20230117204849/https://techcrunch.com/2015/02/25/target-says-credit-card-data-breach-cost-it-162m-in-2013-14/) (以及许多其他的)，人们的证书在互联网黑市上被广泛共享。

谷歌希望帮助解决这个问题，今天在 Google Next 上，它宣布了上下文感知访问，这是一个新的程序，它可以超越你的证书来帮助确定是否真的是你或有人假装是你。

环境感知访问允许管理员定义一组信息，帮助他们更准确地确定试图访问您的服务的人的身份。“上下文感知访问允许组织根据用户的身份、位置和请求的上下文来定义和实施对 GCP API、资源、G Suite 和第三方 SaaS 应用的粒度访问，”谷歌解释道。

更好地了解访问您的服务的人的一种方法是查看一些上下文线索，例如他们在哪里登录，他们从哪里登录的机器的 IP 地址，一天中的时间和其他因素。根据你对这个人的了解，所有这些都有意义吗？

这个想法彻底颠覆了安全责任的概念。它不要求用户完全负责证明他们是谁，而是将责任(和控制权)交给管理员，这样更有意义。

谷歌创造了这个安全工具，因为它和其他公司一样认识到用户不再局限于办公室。他们在移动设备上工作，访问应用程序和云服务，信任身份变得更加困难，尤其是有这么多被盗的凭据。

新程序基于谷歌的 BeyondCorp 愿景(T7 ),这是他们在 2011 年开始开发的一个想法，旨在解决计算不再发生在明确定义的边界内的事实。在移动和云出现之前，人们通常从特定的地方访问计算机系统。如果有人试图从外部登录，你可以抓住他们，把他们赶走。

移动和云改变了这一切，谷歌开始定义一个叫做零信任的概念，即你不信任你服务上的任何人，并基于这个想法建立一个适当的安全位置。身份确实是这个的核心，但是在某些时候，即使是在零信任模型中，你也必须让人们使用你的服务做生意。该工具为零信任模型中的管理员提供了除用户名和密码之外的更多信息，以确定用户是否可信。

如今，使用 VPC 服务控制的客户可以使用上下文感知访问管理。据该公司称，它将很快适用于使用云身份和访问管理(IAM)、云身份感知代理(IAP)和云身份的客户。

[![](img/80e4495f609f54f4cba3339dc07ebec4.png)](https://web.archive.org/web/20230117204849/https://techcrunch.com/tag/google-cloud-next-2018)