# 加密消息应用 Wire 添加用户名，以便您可以限制与联系人共享的内容 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/12/16/encrypted-messaging-app-wire-adds-usernames-so-you-can-limit-what-you-share-with-contacts/>

由 [Skype 联合创始人 Janus Friis](https://web.archive.org/web/20230117202738/https://techcrunch.com/2014/12/02/skype-co-founder-backs-wire-a-new-communications-app-launching-today-on-ios-android-and-mac/) 支持的端到端加密移动通讯应用 [Wire](https://web.archive.org/web/20230117202738/https://play.google.com/store/apps/details?id=com.wire&hl=en) 增加了一个用户名选项，允许人们通过该应用与其他人交流，而无需分享他们的手机号码或电子邮件。

这是备受瞩目的加密消息应用 Signal 仍然缺乏的隐私保护功能，并且[已经因为](https://web.archive.org/web/20230117202738/https://techcrunch.com/2016/11/07/signal-app-maker-rebuts-criticism-of-dev-direction-by-calling-for-more-community-help/)受到了一些批评。脸书旗下的 WhatsApp 于今年 4 月(T6)完成了端到端加密的推广，它也要求用户与所有联系人分享他们的电话号码——随着它向允许企业在平台上建立业务(T9)的方向发展，这可能会导致更多用户在同意添加新联系人之前暂停。

有线用户名在应用程序中是公开的，这对于隐私功能来说似乎是违反直觉的，因为应用程序的用户可以运行大范围的搜索来调出用户名和姓名的列表。尽管不要求网络用户在网络名称或用户名字段中输入真实的全名——这意味着用户可以决定他们对其他人的可见性。

你仍然需要在注册过程中与 Wire 分享你的电话号码或电子邮件，才能使用该应用程序，但不需要与你的所有联系人分享这些个人数据，这与其他一些消息应用程序不同。

两年前，Wire 作为一款桌面应用在手机上推出，去年四月在 T2 将桌面应用扩展为类似 Skype 的网络应用。它现在标榜自己是一个“私人信使”应用程序，标明了最近增加的其他功能，例如可以在 iOS 应用程序上[关闭 CallKit 集成，以避免将你的通话记录数据发送到 iCloud 以及一个](https://web.archive.org/web/20230117202738/https://medium.com/wire-news/ios-2-23-2720-df69dfc7f886#.jj5virn1x)[端到端加密的 bot API](https://web.archive.org/web/20230117202738/https://medium.com/wire-news/wires-end-to-end-encrypted-bot-api-is-coming-861d04825d1#.sjzjnq2my) 。

该应用程序还支持给消息设置一个[计时器——从 5 秒到一天——这样一旦指定的时间段过去，它们就会从聊天日志中消失。](https://web.archive.org/web/20230117202738/https://medium.com/wire-news/safe-and-tidy-with-timed-messages%EF%B8%8F-4f26ff17b11b#.vmt8xnrzx)

据一位发言人称，Wire 的加密技术名为 proteus，它表示这是自己对 OWS 信号协议的实现，因此它可以消除将电话号码用作标识符的需要，并允许其他方法。Wire 还公开了它的代码以增强对其安全声明的信任。

**更新:** OWS 反对 Wire 声称它是建立在信号协议上的，Wire 已经澄清它的加密是建立在 Axolotl 协议上的——信号协议的前身。“在 Wire 推出 E2EE(2016 年 3 月)时，Signal 使用的是 Axolotl 协议，后来他们将其重命名为 Signal 协议，”Wire 发言人表示。然而，OWS 大学的莫邪·马林斯派克是信号协议的作者，他坚持认为美西螈只是其中的一部分。“信号协议由我们开发的许多部分组成，*其中一个*被称为 Axolotl 棘轮，”他告诉 TechCrunch。“后来更新并更名为双棘轮，在此处指定为。因此，他们是正确的，Wire 使用了(旧的、过时的、错误应用的)双棘轮实现作为 Proteus 的一部分，但这只是信号协议的一小部分。Proteus 不是信号协议实现。”

(同样值得注意的是，OWS 之前对 Wire 提出了侵犯版权的指控(T0)，而 Wire [指控(T3)试图勒索许可费(被 OWS 否认)。尽管 Wire 的诉讼后来被撤销了。该公司还同意应马林斯派克的要求在其版权声明中加入一些内容，指定其协议是“*基于 libsignal-protocol-java，由 Open Whisper Systems 提供”)。*](https://web.archive.org/web/20230117202738/http://www.forbes.com/sites/thomasbrewster/2016/05/11/wire-skype-sued-moxie-marlinspike-extortion/#5577d89d3ff5)

除了让用户打电话和分享常见的多媒体组合(文本、图片、音频、视频、位置、gif)之外，它还包括一个向联系人发送 ping 的功能。上面写着所有通过应用程序发送的内容都是端到端加密的。

Wire 是免费下载的，而且目前没有广告，尽管还不清楚它最终的商业模式可能是什么。除了 Friis，这家总部位于瑞士的初创公司还获得了来自 Iconical.com 的投资，投资金额未披露，该公司由工程师、高管和设计师组成，提供非风险投资模式。

这家初创公司没有公布用户数量——只是说它拥有“数百万”用户——但 Google Play 表示，Android 版的 Wire 应用程序已经被下载了 100 万至 500 万次，高于截至 2015 年 4 月的 10 万至 50 万次下载。

作为一个小小的对比，WhatsApp 的 Google Play Android 应用程序目前已获得 10 亿至 50 亿次下载，因此 Wire 显然远远落后于移动通讯类巨头，尽管它比脸书的竞争对手年轻得多，资源也不那么充足。

除了专注于隐私和安全，以及全套多媒体共享选项，Wire 还努力通过设计实现差异化——其界面具有简约、干净的外观和感觉，与许多移动消息应用程序中使用的消息气泡图案有所不同。