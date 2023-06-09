# PaaS 到底怎么了？

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/04/11/whatever-happened-to-paas/>

乔恩·埃文斯是工程咨询公司 HappyFunCorp 的首席技术官；六部小说、一部漫画小说和一本游记的获奖作者；自 2010 年以来一直是 TechCrunch 的周末专栏作家。

More posts by this contributor

2009 年，我发现了谷歌应用引擎并爱上了它。它的承诺是:任何软件开发人员都可以构建可供任何人、任何地点、任何时间使用的 web 应用程序，而不必担心服务器配置、数据库设置、操作系统版本、安全补丁、负载平衡或伸缩性。*自动缩放！我们所要做的就是编写我们的代码；应用引擎将处理其他一切。*

在 2009 年，我觉得很明显，到 2015 年，绝大多数 web 代码都将运行在类似的平台上。谁想和配置和运营较劲？系统管理员将最终从他们令人疲惫的束缚中解放出来。(我的意思是:变成开发者，被平台提供商雇佣，或者被解雇。)最后，我们将可以自由地编写代码，而不必担心代码是如何执行的或者在哪里执行的。天平将从我们眼前落下，我们将从操作链中解放出来，我们的未来将是光明的，没有实施细节。

…是的，所以事情并不完全是这样。

为什么不呢？

这是没有“[写一次，到处跑](https://web.archive.org/web/20230306001059/http://en.wikipedia.org/wiki/Write_once,_run_anywhere)”App Engine 实际上实现了，并将继续实现最初的承诺。(而且[多了](https://web.archive.org/web/20230306001059/https://cloud.google.com/appengine/features/)，这也是我为什么还在我的[侧](https://web.archive.org/web/20230306001059/http://www.scanvine.com/) [项目](https://web.archive.org/web/20230306001059/http://www.vortext.co/)使用 App Engine 的原因。)当然，你用它换来了一大堆星号和小字、“爆炸式索引”和“碎片计数器”，以及偶尔令人费解的内存泄漏和等待时间；但正如一位谷歌朋友曾经说过的，“App Engine 相当神奇，它对每个用户来说运行速度都一样慢，不管用户有多少。”

还有很多其他平台即服务(PaaS)的竞争者。甚至亚马逊，这个无可争议的愚蠢的虚拟计算基础设施之王，也提供了 PaaS 和它的弹性豆茎。我经常专业地使用 [Heroku](https://web.archive.org/web/20230306001059/https://www.heroku.com/) ，你知道吗，它们也非常棒:在异步任务或自动负载平衡方面不如 App Engine，但在 git-push-to-deploy 和 PostgreSQL 数据库方面要好得多，并且，嗯，没有提供在其他地方完全没有的 API。谷歌的 API 通常比其他任何地方的都要好。这就是在(或多或少)谷歌自己的平台上运行代码的得失

–但就连谷歌自己似乎也不像 2009 年那样热衷于这个概念。2012 年，大概是对 App Engine 的成功不满，他们推出了[谷歌计算引擎](https://web.archive.org/web/20230306001059/https://cloud.google.com/compute/)，这是亚马逊网络服务的直接竞争对手。当然，这两种方式都比购买和提供自己的服务方便得多；但是从易用性、灵活性和开发时间方面来看，这两者似乎都比 PaaS 有明显的退步。为什么我错了？为什么 PaaS 没有征服一切？

它取得了成功。Snapchat，[著名的](https://web.archive.org/web/20230306001059/https://techcrunch.com/2014/02/18/snapchat-hires-googler-pisses-off-his-googler-friends/)，运行在 App Engine 之上， [Khan Academy](https://web.archive.org/web/20230306001059/https://cloud.google.com/customers/khan-academy/) 也是如此。 [Genius](https://web.archive.org/web/20230306001059/https://techcrunch.com/2013/02/14/heroku-admits-to-performance-degradation-over-the-past-3-years-after-criticism-from-rap-genius/) 和[产品搜索](https://web.archive.org/web/20230306001059/https://www.heroku.com/customers/producthunt)在 Heroku 上运行。这两个城市还拥有无数其他初创公司和更成熟的公司。但如果 PaaS 更成功，谷歌就不会为计算引擎费心了。如果 PaaS 更成功，Docker 就不会成为新的热门。如果 PaaS 更成功，DevOps 将不再是一个东西。

那么，为什么人们仍然在开发和建立他们自己的 AWS 和计算引擎实例呢？为什么 App Engine 和 Heroku 和 Elastic Beanstalk 没有征服所有？细粒度控制真的那么重要吗？

我怀疑原因有三:成本、锁定和文化。

App Engine 的[价格](https://web.archive.org/web/20230306001059/https://cloud.google.com/appengine/pricing)定期下降，但它们数量庞大且令人困惑，单个实例——一个相当小的虚拟机——每天的成本超过一美元，还不算存储或带宽。同样适用于 [Heroku](https://web.archive.org/web/20230306001059/https://www.heroku.com/pricing) 。您只需购买并运行自己的服务器，就能获得更高的性价比。您还会遇到更大的麻烦，开发时间会明显变慢；但对许多人来说，这种权衡是不值得的。

然后就是锁定。一旦你在 App Engine 的自定义 API 上构建了你的应用程序，你就已经承诺了；没有简单的方法可以放弃，去找另一个供应商。对于其他 PaaS 提供商来说，这种束缚较少，但仍然存在。没有通用的 PaaS 等同于事实上的 IaaS(基础设施即服务)标准，如 [OpenStack](https://web.archive.org/web/20230306001059/http://en.wikipedia.org/wiki/OpenStack) 或 [Docker](https://web.archive.org/web/20230306001059/http://en.wikipedia.org/wiki/Docker_%28software%29) 。

第三个，也是最站不住脚的，也可以说是最有力的原因是文化。公司不想放弃对其系统的感知控制，即使这种控制永远不值得其相关的复杂性，可以理解的是，系统管理员也不想让自己脱离工作。

然而，这三个不去 PaaS 的理由都是暂时的。成本持续下降。文化在不断变化。而且有迹象表明[向可互换的 PaaS 服务和标准缓慢迈进](https://web.archive.org/web/20230306001059/https://cloud.google.com/appengine/docs/managed-vms/)。(你可能会说 Docker 本身就是朝着这个方向迈出的一大步。)

在电力出现的早期，工厂都有自己的发电机；然后，最终，他们转移到网格。IaaS 相当于每家公司从电网中获取原始电力，但用自己的变压器降压，并在内部从三相转换为单相。我怀疑我们仍然在走向一个很大程度上是 PaaS 的世界，在这个世界中，服务器代码大部分只是运行，而开发人员不知道或不关心有问题的服务器。只是比我希望的要慢一点。