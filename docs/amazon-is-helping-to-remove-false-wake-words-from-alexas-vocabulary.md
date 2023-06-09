# 亚马逊正在帮助从 Alexa 的词汇表中删除错误的 wake 单词 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/05/15/amazon-is-helping-to-remove-false-wake-words-from-alexas-vocabulary/>

# 亚马逊正在帮助从 Alexa 的词汇中删除虚假的 wake 单词

亚马逊的智能助手已经非常擅长识别自己的名字(让许多分享它的人明显懊恼的是),但这并不能使它免于误报。为了让 Alexa 更好地过滤掉类似的单词，亚马逊今天推出了一项名为[基于云的唤醒单词验证](https://web.archive.org/web/20221024050613/https://developer.amazon.com/blogs/alexa/post/b136b3e7-0ba8-4589-aaf9-2a037fc4e9c9/cloud-based-wake-word-verification-improves-alexa-wake-word-accuracy-on-your-avs-products)的新功能，适用于在其设备中内置 Alexa 的第三方制造商。

这将使他们的设备更加可靠，并且与亚马逊自己的 Echo 产品线相比更具竞争力，后者目前使用类似的系统来避免误报。

新功能利用了一种双因素语音识别系统。第一步和之前一样，用硬件(Echo，Echo Dot 等。)处理初始检测。然而，在此之后，该词将通过基于云的过程进行二次验证，以检查误报。如果检测到一个，唤醒词验证将指示硬件关闭音频流。

这种额外的处理不会减慢 Alexa 的响应时间，而是会使与 Alexa 的交互不那么令人讨厌，因为她不会意外地回答你从未问过的问题。

此次更新向[解决日益增长的关于 Echo 在家中的隐私问题](https://web.archive.org/web/20221024050613/https://beta.techcrunch.com/2017/02/23/alexa-free-speech/)迈出了一小步。智能家居中枢设计有一个永远在线的麦克风来监听它的唤醒词——当把这些设备带到我们家中一些最隐私的地方时，这是一个特别的问题。

亚马逊最近解决了这一问题，告诉 TechCrunch:“Echo Look 使用与 Echo 相同的设备上关键词定位，来检测唤醒词，并且只检测唤醒词。当检测到唤醒词时，光环会变成蓝色，表明 Alexa 正在向 AWS 云传输音频。”

这项新功能有望减少误报，并在系统从唤醒模式转换到被动监听模式时关闭蓝色 LED。

第三方硬件开发商将不得不调整他们的系统，以启用新功能。目前，[最近发布的 Ecobee4](https://web.archive.org/web/20221024050613/https://beta.techcrunch.com/2017/05/03/ecobee-is-building-alexa-into-its-thermostats-and-light-switches/) 是唯一一款启用该功能的设备。智能恒温器代表了 Alexa 开发者的转变。该系统不是简单地加入语音功能，而是兼作一种代理壁挂式回声。

这种第三方支持，加上一些新宣布的回应，很可能只会增加这类设备的隐私问题。今天的声明标志着解决这一问题的一小步。然而，这将对任何推出[现实生活回音银](https://web.archive.org/web/20221024050613/https://beta.techcrunch.com/2017/05/13/snl-just-came-up-with-a-hilarious-version-of-alexa-designed-for-senior-citizens/)的计划造成一点阻碍。