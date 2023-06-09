# 用户在了解到 AccuWeather iPhone 应用程序将位置数据发送给第三方后，会转储该应用程序 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/08/22/accuweather-revealmobile-ios/>

AccuWeather 的 iOS 应用程序可能有猫腻。安全研究员 Will Strafach 在 Medium 上发布了一个关于热门天气应用行为[的警告，用户似乎正在关注。](https://web.archive.org/web/20221016030915/https://medium.com/@chronic_9612/advisory-accuweather-ios-app-sends-location-information-to-data-monetization-firm-83327c6a4870)

根据 Strafach 的 Medium post，AccuWeather 应用程序请求用户的位置许可，不是提供定制的基于位置的天气数据，而是向一家名为 RevealMobile 的第三方公司发送一些非常具体的地理数据。这包括:

> *   “你的精确 GPS 坐标，包括当前速度和高度。
> *   您当前连接的 Wi-Fi 路由器的名称和“BSSID ”,可用于通过各种在线服务进行地理定位。
> *   您的设备是否打开了蓝牙。"

值得注意的是，关闭 AccuWeather 的位置数据并没有限制该应用的覆盖范围。正如 Strafach 的 Medium post 所指出的，“如果您不允许 AccuWeather 访问您的 GPS 信息，它仍会发送您的 Wi-Fi 路由器名称和 BSSID，提供对有关您设备所在位置的不太精确的位置信息的公开移动访问。另一家公司的这种做法似乎已经引起了联邦贸易委员会的注意。

RevealMobile 似乎专注于移动收入和利用位置数据进行广告定位。该公司在其主页上的一篇博客文章中解释道:“价值在于了解消费者的路径以及他们一天去了哪里。”。“从家到工作单位、从零售到足球训练再到晚餐的旅行对于了解客户至关重要，代表着移动位置数据的新机遇。”

对于任何有隐私意识的人来说，这种做法可能不会感到震惊，但仍然令人不安。AccuWeather 是一款受欢迎的预测应用，用户可能会信任它将自己的位置用于与天气相关的目的，而不是第三方数据销售。正如 Strafach 所指出的，AccuWeather 并不是唯一一个因为不透明而分享这种跟踪数据的公司。尽管如此，这并没有改变糟糕的隐私政策——也没有让用户在 Twitter 上表达他们的愤怒有任何减少。

TechCrunch 已联系 AccuWeather 获取更多信息，并将随着事态的发展更新报道。

更新:AccuWeather 向 TechCrunch 发送了以下声明。

> 尽管与实际信息不相关的来源提供了相反的故事，但如果用户选择退出 AccuWeather 上的位置跟踪，在没有用户进一步选择加入许可的情况下，不会收集或传递 GPS 坐标。
> 
> 其他数据，如不属于用户信息的 Wi-Fi 网络信息，在 Reveal SDK 上短期可用，但 AccuWeather 未使用。事实上，AccuWeather 并不知道这些数据可供其使用。因此，AccuWeather 从未将这些数据用于任何目的。
> 
> AccuWeather 和 Reveal Mobile 致力于遵循行业标准和最佳实践。我们也认识到这是一个快速发展的领域，某一天的最佳实践可能会改变第二天。因此，我们致力于定期更新我们的实践。
> 
> 为了避免任何进一步的误解，在 Reveal 更新其 SDK 时，AccuWeather 将从其 iOS 应用程序中删除 Reveal SDK，直到它完全符合相应的要求。一旦恢复，最终结果应该是当有人选择退出位置共享时，零数据传输回揭示移动。与此同时，AccuWeather 已经禁用了 SDK，等待 SDK 的移除以及随后的恢复。
> 
> Reveal 声明 SDK 可能会被误解，他们保证没有通过他们收集的任何信息进行位置的逆向工程，这也不是他们的意图。
> 
> AccuWeather 将更新其实践、通信和 ULAs，使其透明并符合不断发展的标准。AccuWeather 和 Reveal 继续改进数据处理方法，努力提供卓越、无缝和安全的用户体验。
> 
> 我们很高兴有一个支持性的社区，它强调了我们可以优化和更加透明的领域。