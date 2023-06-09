# Nvidia 推出新的 Drive Constellation 模拟自动驾驶测试系统

> 原文：<https://web.archive.org/web/https://techcrunch.com/2018/03/27/nvidia-debuts-new-drive-constellation-simulated-self-driving-test-system/>

# 英伟达推出新的 Drive Constellation 模拟自动驾驶测试系统

Nvidia 已经将 AutoSIM 虚拟环境用于测试它最初在 CES 上展示的自动驾驶汽车，将其与 Drive Pegasus AI 车载计算机相结合，并创建了一个虚拟测试和验证循环，可以在超现实环境中处理数十亿虚拟驾驶里程，能够模拟边缘情况，并重现难以在真实道路上彻底测试的条件。

为其合作伙伴设计的系统名为 Drive Constellation，涉及使用两种不同的服务器在完全虚拟化的环境中准确模拟真实世界的自动驾驶。一台服务器运行英伟达的 Drive Sim 软件，该软件将模拟自动车辆在道路上的感官体验，提供逼真的相机捕捉和来自虚拟化激光雷达和雷达系统的数据，精确模拟在真实道路上驾驶时捕捉的内容。

系统中的第二台服务器运行的是 Nvidia Drive Pegasus AI，即自动驾驶汽车的“大脑”,它处理第一台服务器提供的数据，就像它是从道路上捕获的车辆传感器提供的真实数据一样。然后，由飞马座驱动的服务器将其控制命令返回给模拟器，告诉它进行驾驶活动，就像它在路上驾驶一辆真正的汽车一样。

这就是英伟达所谓的“硬件在环”周期，它可以每秒钟进行 30 次这样的交换，有助于验证自动驾驶软件的性能。因为它可以完全由测试人员控制，所以可以调整等式中的 Drive Sim 部分，以提供真实的驾驶体验，就像人们可能在道路上遇到的一样，或者像忍受 24 小时眩目的人工条件，中午的峰值太阳，或者研究人员或开发人员可能想要测试和优化的任何边缘情况。

边缘情况仍然是任何开发自动驾驶汽车的人的主要关注点，依赖真实世界的测试来构建可以正确处理这些边缘情况的软件的问题是，它们不经常发生，也很难复制。软件模拟是为这些很少发生的情况做准备的一种方式，没有风险，也不必等待条件自动调整到正确(或错误，视情况而定)。

Nvidia 的 Drive Constellation 将在今年第三季度通过早期访问开始向其一些合作伙伴提供，并将在此后的某个时间推出商业产品。当然， [Nvidia 今天也宣布，在调查最近导致行人死亡的](https://web.archive.org/web/20230317220124/https://techcrunch.com/2018/03/27/nvidia-reportedly-suspending-all-autonomous-vehicle-testing/)[优步自动驾驶汽车测试事故](https://web.archive.org/web/20230317220124/https://techcrunch.com/2018/03/19/uber-self-driving-test-car-involved-in-accident-resulting-in-pedestrian-death/)期间，它将暂时停止其自动驾驶测试，但理论上，更多的模拟测试将减少真实道路上的潜在事故。