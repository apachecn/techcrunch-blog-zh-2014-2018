# 区块链开源迅雷网络，为即时比特币交易铺路 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/05/16/blockchain-open-sources-thunder-network-paving-the-way-for-instant-bitcoin-transactions/>

[区块链](https://web.archive.org/web/20220924184804/https://www.blockchain.com/)，世界上最受欢迎的比特币钱包[背后的公司，一直在](https://web.archive.org/web/20220924184804/https://beta.techcrunch.com/2014/10/07/blockchain-goes-from-bootstrapping-to-scoring-30-million/)[悄悄进行一个叫做雷霆](https://web.archive.org/web/20220924184804/https://blog.blockchain.com/2016/05/16/announcing-the-thunder-network-alpha-release)的有趣项目。Thunder network 是一个替代性的节点网络，让你在几秒钟内完成非链比特币支付，并不时回到比特币区块链进行结算。这让我再次对比特币感到兴奋。

这听起来很复杂，但它非常简洁，可能是比特币交易的一项强大创新。但首先，让我们后退一步。

如果你曾经尝试过从一个钱包向另一个钱包发送几个比特币，你知道在区块链确认交易之前可能需要 10 到 20 分钟。

这背后的原因是区块链是一个共享相同交易记录的服务器网络。当您发送两个比特币时，区块链中的所有节点都将在此交易中写入一行，以便每个人都可以确认发起钱包丢失了两个比特币，而目的钱包现在有两个额外的比特币。

这太棒了，这就是比特币完全去中心化的原因。但它也很慢，难以扩展，而且价格昂贵。

去年，Joseph Poon 和 Thaddeus Dryja [写了一篇关于比特币的可扩展性和速度问题的论文](https://web.archive.org/web/20220924184804/https://lightning.network/lightning-network-paper.pdf)，并定义了闪电网络。这些替代网络将独立于主要的比特币区块链运行，能够在一秒钟内注册交易。它使用智能合同，因此闪电网络中的所有节点都不需要知道所有的交易。

然而，这都是理论。区块链聘请了 Mats Jerratsch，并开始致力于一种闪电网络的实现。这就是该公司今天宣布并开放源代码的内容。 [Thunder](https://web.archive.org/web/20220924184804/https://www.blockchain.com/thunder) 是第一个类似闪电的网络实现。区块链已经在运行迅雷节点，其他比特币公司可以查看源代码，提供迅雷钱包，采用这个网络或分叉它。迅雷还可以与其他加密货币配合使用。而创业公司让[成为迅雷](https://web.archive.org/web/20220924184804/https://blog.blockchain.com/2016/05/16/transaction-0/)上的第一笔直播交易。

虽然 Blockchain 还不会为区块链钱包用户使用 Thunder，但这家初创公司已经在考虑像 Thunder 这样的解决方案在现实生活中的优势。

![Screen Shot 2016-05-16 at 3.41.47 PM](img/3834254b51eeeed2a6ed95aa537a887d.png)

有了迅雷，一笔交易的速度非常快，网络每秒可以处理 10 万笔交易。平均而言，Visa 每秒处理 2000 笔交易，Visa 网络每秒能够处理[56000 笔交易](https://web.archive.org/web/20220924184804/https://usa.visa.com/dam/VCOM/download/corporate/media/visa-fact-sheet-Jun2015.pdf)。

从这个角度来看，区块链钱包用户今年有望进行 4000 万笔交易，或每秒约 1.3 笔交易。令人印象深刻，但说实话。尽管有许多其他钱包，但鉴于区块链是最受欢迎的钱包制造商，比特币的交易量远远落后于 Visa。出现这种情况的原因是比特币交易已经过于繁琐。所以我相信像迅雷这样的项目是解决方案的一部分。

同样重要的是，由于迅雷，交易变得便宜得多。当你将迅雷支付的款项返还给比特币区块链时，仍会涉及区块链费用。但是在回到区块链之前，你可以进行很多很多的迅雷交易——而且迅雷交易不会涉及很多节点。如果你将费用除以迅雷交易的次数，使用比特币支付会便宜得多。费用如此之低，以至于你终于可以想象使用比特币进行微交易了。

因此，迅雷将使比特币成为 Visa 的可行替代品。它消除了现有比特币协议背后的许多限制。

现在，仍然存在一些障碍。迅雷目前还不能与任何拥有比特币钱包的人合作，因为比特币核心开发团队需要发布[隔离见证](https://web.archive.org/web/20220924184804/https://bitcoincore.org/en/2016/01/26/segwit-benefits/)和[检查序列验证](https://web.archive.org/web/20220924184804/https://github.com/bitcoin/bips/blob/master/bip-0112.mediawiki)功能。但好消息是，这些功能已经在路线图上，核心团队希望让闪电网络成为可能。在此之前，迅雷依赖于可信节点。但随着未来比特币的更新，雷霆可以成为一个全面的闪电网络。

Thunder 是一个令人兴奋的项目，可能会彻底改变比特币的一些使用案例。由于比特币的局限性，许多人转向了替代加密货币，如 [Ether](https://web.archive.org/web/20220924184804/https://en.wikipedia.org/wiki/Ethereum) 。缓慢但肯定的是，比特币社区正在迎头赶上，并使比特币支付更具吸引力。