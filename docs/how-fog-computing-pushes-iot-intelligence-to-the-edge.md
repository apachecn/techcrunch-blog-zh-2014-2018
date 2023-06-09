# 雾计算如何将物联网智能推向边缘

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/08/02/how-fog-computing-pushes-iot-intelligence-to-the-edge/>

本·迪克森是一名软件工程师，也是

[TechTalks](https://web.archive.org/web/20230316161016/https://bdtechtalks.com/)

.

More posts by this contributor

随着物联网演变为万物互联，[将其触角延伸到几乎每个领域](https://web.archive.org/web/20230316161016/https://bdtechtalks.com/2016/05/10/iot-and-machine-learning-are-invading-our-lives-is-it-a-good-thing/)，高速数据处理、分析和更短的响应时间变得比以往任何时候都更加必要。通过当前支持物联网系统的集中式、基于云的模型来满足这些要求有些问题，但通过[雾计算](https://web.archive.org/web/20230316161016/http://internetofthingsagenda.techtarget.com/definition/fog-computing-fogging)可以实现，这是一种分散式架构模式，[将计算资源和应用服务带到更靠近边缘的地方](https://web.archive.org/web/20230316161016/https://bdtechtalks.com/2016/07/19/how-iot-can-benefit-from-cloud-computing/)，这是数据源和云之间连续体中最合理、最高效的地方。

由思科创造的术语“雾计算”指的是将云计算的优势和能力带到数据生成和处理的地方。雾计算减少了传输到云进行处理和分析的数据量，同时还提高了安全性，[这是物联网行业的一个主要关注点](https://web.archive.org/web/20230316161016/https://techcrunch.com/2015/10/24/why-iot-security-is-so-critical/)。

以下是从云到雾的过渡如何帮助应对物联网行业当前和未来的挑战。

## 云的问题是

物联网的爆炸式增长归功于物理事物和操作技术(oT)与分析和机器学习应用程序的连接，这些应用程序可以帮助从设备生成的数据中收集见解，并使设备能够在没有人工干预的情况下做出“智能”决策。目前，此类资源主要由云服务提供商提供，他们拥有计算和存储能力。

然而，尽管云模型功能强大，但它并不适用于运营时间要求苛刻或互联网连接不畅的环境。在远程医疗和病人护理等场景中尤其如此，在这些场景中，几毫秒就可能产生致命的后果。车对车的通信也是如此，在这种情况下，碰撞和事故的预防无法承受往返云端服务器所带来的延迟。云范式就像让你的大脑在几英里之外指挥你的四肢——在你需要快速反应的地方，它不会帮你。

> 云范式就像让你的大脑在几英里之外指挥你的四肢。

此外，让每台设备都连接到云并通过互联网发送原始数据可能会带来[隐私、安全和法律影响](https://web.archive.org/web/20230316161016/https://bdtechtalks.com/2016/04/20/why-do-we-need-to-take-iot-security-more-seriously/)，尤其是在处理敏感数据时，这些数据在不同国家/地区受到[不同法规的约束](https://web.archive.org/web/20230316161016/http://www.zdnet.com/article/privacy-laws-how-the-us-eu-and-others-protect-iot-data-or-dont/)。

## 雾放在了完美的位置

物联网节点更接近行动，但就目前而言，它们不具备执行分析和机器学习任务的计算和存储资源。另一方面，云服务器有马力，但距离太远，无法及时处理数据和做出响应。

雾层是一个完美的结合点，其中有足够的计算、存储和网络资源来模拟边缘的云功能，并支持本地数据摄取和结果的快速周转。

IDC 的一项[研究估计，到 2020 年，全球 10%的数据将由边缘设备产生。这将进一步推动对更高效的雾计算解决方案的需求，同时提供低延迟和整体智能。](https://web.archive.org/web/20230316161016/https://www.emc.com/collateral/analyst-reports/idc-digital-universe-united-states.pdf)

雾计算有自己的支持机构 [OpenFog Consortium](https://web.archive.org/web/20230316161016/http://www.openfogconsortium.org/) ，成立于 2015 年 11 月，其使命是推动雾计算架构的行业和学术领导力。该联盟提供参考架构、指南、样本和 SDK，帮助开发人员和 IT 团队了解雾计算的真正价值。

思科、戴尔和英特尔等主流硬件制造商已经开始与物联网分析和机器学习供应商合作，提供支持雾计算的物联网网关和路由器。一个例子是思科最近收购了[物联网分析公司 ParStream](https://web.archive.org/web/20230316161016/http://www.rtinsights.com/with-parstream-cisco-thinks-edge-analytics/) 和[物联网平台提供商 Jasper](https://web.archive.org/web/20230316161016/http://investor.cisco.com/investor-relations/news-and-events/news/news-details/2016/Cisco-Announces-Intent-to-Acquire-Jasper-Technologies-Inc/default.aspx) ，这将使这家网络巨头在其网络设备中嵌入更好的计算能力，并在雾计算最为关键的企业物联网市场中占据更大份额。

分析软件公司也在扩展产品，并为边缘计算开发新工具。 [Apache Spark](https://web.archive.org/web/20230316161016/http://spark.apache.org/) 是一个基于 [Hadoop](https://web.archive.org/web/20230316161016/http://hadoop.apache.org/) 生态系统的数据处理框架的例子，适用于边缘生成数据的实时处理。

> 通过云获得的洞察力可以帮助在雾层更新和调整策略和功能。

物联网行业的其他主要参与者也在押注雾计算的增长。微软的 [Azure IoT](https://web.archive.org/web/20230316161016/https://azure.microsoft.com/en-us/suites/iot-suite/) 是领先的企业物联网云平台之一，旨在通过推动其 Windows 10 物联网成为物联网网关和其他高端边缘设备的首选操作系统，确保其在雾计算中的主导地位，这些设备将成为雾计算的核心焦点。

## 雾消除了云吗？

雾计算提高了效率，减少了需要发送到云端进行处理的数据量。但它是为了补充云，而不是取代云。

云将继续在物联网周期中发挥重要作用。事实上，随着雾计算在边缘承担短期分析的负担，云资源将被释放出来承担更重的任务，特别是在历史数据和大型数据集的分析方面。通过云获得的洞察力可以帮助在雾层更新和调整策略和功能。

在很多情况下，云的集中式高效计算基础设施在性能、可扩展性和成本方面都优于分散式系统。这包括需要分析大量分散来源的数据的环境。

正是雾和云计算的结合将加速物联网的采用，尤其是对企业而言。

## 雾计算有哪些用例？

雾计算的应用很多，它正在为物联网生态系统的关键部分提供动力，特别是在工业环境中。

由于雾计算的力量，总部位于纽约的可再生能源公司 [Envision](https://web.archive.org/web/20230316161016/http://www.envision-energy.net/) 已经能够从其运营的巨大风力涡轮机网络中获得 15%的生产率提高。

该公司一次处理多达 20tb 的数据，这些数据由安装在它管理的 20，000 台涡轮机上的 300 万个传感器生成。将计算转移到边缘使 Envision 能够将数据分析时间从 10 分钟缩短到几秒钟，为他们提供可操作的见解和显著的业务优势。

物联网公司 Plat One 是另一家使用雾计算来改善其管理的 100 多万个传感器的数据处理的公司。该公司使用 ParStream 平台发布数十万台设备的实时传感器测量结果，包括智能照明和停车、港口和交通管理以及由 5 万台咖啡机组成的网络。

雾计算在智慧城市也有几个用例。在加利福尼亚州的帕洛阿尔托[，一个 300 万美元的项目将使交通灯与联网车辆](https://web.archive.org/web/20230316161016/http://www.govtech.com/fs/Is-Edge-Computing-Key-to-the-Internet-of-Things.html)集成，有望创造一个未来，人们不会无缘无故地在空无一人的十字路口等车。

在交通领域，它通过提供实时分析和驾驶模式决策，帮助半自动驾驶汽车在[帮助司机避免分心和偏离道路](https://web.archive.org/web/20230316161016/http://www.wired.com/brandlab/2016/03/how-semi-autonomous-vehicles-are-helping-to-power-a-potentially-safer-future-on-the-road/)。

它还可以帮助减少由警察仪表板和摄像机产生的大量音频和视频记录的传输。[配备边缘计算功能的摄像机](https://web.archive.org/web/20230316161016/http://eecatalog.com/medical/2015/04/28/edge-computing-brings-performance-to-the-heterogeneous-iot/)可以实时分析视频，只在必要时将相关数据发送到云端。

## 雾计算的未来是怎样的？

目前的趋势表明，随着物联网的扩展和征服新的领域，雾计算的使用和重要性将继续增长。随着廉价、低功耗的处理和存储变得更加可用，我们可以预计计算将更加接近边缘，并在生成数据的相同设备中变得根深蒂固，从而为设备间智能和交互创造更大的可能性。只记录数据的传感器可能有一天会成为历史。