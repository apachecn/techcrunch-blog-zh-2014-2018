# 谷歌云平台将图形处理器的价格降低了 36%

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/11/20/google-cloud-platform-cuts-the-price-of-gpus-by-up-to-36-percent/>

# 谷歌云平台将图形处理器的价格降低了 36%

谷歌今天[宣布](https://web.archive.org/web/20230327164516/https://cloudplatform.googleblog.com/2017/11/new-lower-prices-for-GPUs-and-preemptible-Local-SSDs.html)将通过其计算引擎削减使用英伟达特斯拉 GPU 的[的价格，降幅高达 36%。在美国地区，使用稍微旧一点的 K80 GPUs 现在每小时将花费 0.45 美元，而使用更新更强大的](https://web.archive.org/web/20230327164516/https://cloud.google.com/compute/docs/gpus/) [P100](https://web.archive.org/web/20230327164516/http://www.nvidia.com/object/tesla-p100.html) 机器每小时将花费 1.46 美元(所有这些都是按照[每秒计费](https://web.archive.org/web/20230327164516/https://techcrunch.com/2017/09/26/following-aws-google-compute-engine-also-moves-to-per-second-billing/))。

该公司还将可抢占的本地固态硬盘的价格降低了近 40%。“[可抢占本地固态硬盘](https://web.archive.org/web/20230327164516/https://cloud.google.com/compute/quotas#disk_quotas)”指的是附属于谷歌可抢占虚拟机的本地固态硬盘。不过，你不能将 GPU 附加到可抢占的实例，所以这是一个不错的小奖励声明——但它不会直接让 GPU 用户受益。

至于新的 GPU 定价，很明显，谷歌将这一功能瞄准了那些希望在其云上运行自己的机器学习工作负载的开发人员，尽管还有许多其他应用程序——包括物理模拟和分子建模——极大地受益于这些 GPU 上现有的数百个内核。例如，在谷歌云平台上仍处于测试阶段的 P100 拥有 3594 个内核。

开发人员可以为每个实例附加多达四个 P100 和八个 K80 骰子。像普通虚拟机一样，GPU 用户也将获得持续使用折扣，尽管大多数用户可能不会让他们的 GPU 运行整整一个月。

鉴于 AWS 即将举行的年度开发者大会，很难不看到这一宣布，该大会将在下周占据拉斯维加斯的大部分酒店会议空间。预计 AWS 将发布一些人工智能和机器学习公告，我们也有可能看到 AWS 的一些降价。