# 为什么图像识别即将改变商业 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2016/04/30/why-image-recognition-is-about-to-transform-business/>

肯·韦纳是

[GumGum](https://web.archive.org/web/20230205235834/http://gumgum.com/)

.

在脸书最近的年度开发者大会上，马克·扎克伯格概述了社交网络的人工智能(AI)计划“建立比人类感知更好的系统”然后，他展示了一项令人印象深刻的盲人图像识别技术，可以“看到”图片中发生的事情，并大声解释出来。

从帮助视力受损者的程序和检测大型动物的汽车安全功能，到自动组织未标记的照片集和从社交共享图片中提取商业见解，[图像识别](https://web.archive.org/web/20230205235834/http://venturebeat.com/2015/12/22/2015-was-an-impressive-year-for-image-recognition-check-out-these-milestones/)或计算机视觉的好处才刚刚开始进入这个世界——但它们正在以越来越多的频率和深度这样做。

即将到来的 [LDV 视觉峰会](https://web.archive.org/web/20230205235834/http://www.ldv.co/visionsummit/)已经是第三年了，这是一个致力于所有视觉技术的年度会议，从虚拟现实和相机到医学成像和内容分析。“这些天来，计算机视觉的进步为分析图像创造了巨大的新机会，这些图像正以指数级的速度影响着从汽车到广告到增强现实的每个商业垂直领域，”组织此次峰会的 LDV Capital 的埃文·尼塞尔森表示。

与其他形式的人工智能一样——自然语言处理、生物信息学、游戏——计算机视觉领域从开源、深度学习技术、用户友好的编程工具以及更快、更实惠的计算的扩展中受益匪浅。

许多标题都提到深度学习和人工智能是下一个大事件，但这些不同的工具到底是如何工作的，企业是如何利用它们向世界提供图像技术的？谷歌的 TensorFlow 和脸书的 DeepFace 或者微软的 Project Oxford 是一回事吗？不完全是。为了帮助澄清事情，这里有一个当前图像技术工具的快速分类，以及企业如何使用它们。

## 培训材料:开放数据

得益于[深度学习](https://web.archive.org/web/20230205235834/http://msp.imirus.com/Mpowered/book/vds2016/i4/p52)技术，一种大致模仿人脑的机器学习技术，计算机可以被教会比以往更快地准确识别图片中的内容——但它们需要大量的数据来做到这一点。

进入 [ImageNet](https://web.archive.org/web/20230205235834/http://www.image-net.org/) 和 [Pascal VOC](https://web.archive.org/web/20230205235834/http://host.robots.ox.ac.uk/pascal/VOC/) 。经过多年的制作，这些庞大的免费数据库包含数百万张图片，这些图片标有关于图片内容的关键词——从猫和山到比萨饼和体育活动。这些开放数据集是机器学习图像的基础(计算机能够准确识别照片中的猫的唯一方法是因为它们已经通过分析数百万张标有“猫”字样的照片了解了猫的样子)。

ImageNet 因其年度[视觉识别挑战](https://web.archive.org/web/20230205235834/http://www.engadget.com/2014/08/19/computer-vision/)而闻名于世，由斯坦福和普林斯顿的计算机科学家于 2009 年推出，有 8 万张标记图像。自那以后，它已经发展到包括超过 1400 万张标记图像，其中任何一张都可以在任何时候用于机器训练目的。

在英国各大学的支持下，帕斯卡尔·挥发性有机化合物(Pascal VOC)的图片越来越少，但每一张都有更丰富的注释。这提高了机器学习的准确性和广度，对于某些应用来说，还加快了整个过程，因为它允许省略繁琐的计算机子任务。

> 不是每家公司都有资源或想投资这些资源来建立计算机视觉工程团队。

现在，从谷歌和脸书到初创公司和大学，每个人都使用这些开源图片集来喂养他们的机器学习动物，但大型科技公司有优势从谷歌照片和脸书等应用程序中获取数百万用户标记的图像。你有没有想过为什么谷歌和脸书让你免费上传这么多照片？这是因为这些图片被用来训练他们的深层学习网络变得更加准确。

## 构建模块:开源软件库和框架

一旦你有了数据，是时候制造一台可以从中学习的机器了。进入开源软件库。这些框架可以自由使用，可以作为构建机器学习系统的起点，为不同类型的计算机视觉功能提供服务，从面部和情感识别到医学筛查和汽车中的[大障碍物(read: deer)检测](https://web.archive.org/web/20230205235834/https://www.cars.com/articles/man-or-moose-volvos-large-animal-detection-decides-avoids-1420684261918/)。然后，这些机器学习系统会从 ImageNet 及其同类网站、专有图像(也称 Google Photos)或其他来源(如[匿名索引临床记录](https://web.archive.org/web/20230205235834/https://www.zebra-med.com/))获得图片。

谷歌 [TensorFlow](https://web.archive.org/web/20230205235834/https://www.tensorflow.org/) 是其中一个更知名的库，如果仅仅是因为它在去年底开放源代码时被广泛覆盖的话。TensorFlow(其中一些仍归谷歌所有)被用来开发该公司的许多人工智能项目，从自动驾驶汽车和翻译到谷歌现在和谷歌照片。

但是 TensorFlow 并不是第一个——或者说是唯一一个——开源框架。加州大学伯克利分校的[咖啡馆](https://web.archive.org/web/20230205235834/http://caffe.berkeleyvision.org/)自 2009 年就已经存在，并因其易定制性和庞大的创新群体而广受欢迎，更不用说被 [Pinterest](https://web.archive.org/web/20230205235834/https://engineering.pinterest.com/blog/introducing-new-way-visually-search-pinterest) 和 [Yahoo！/Flickr](https://web.archive.org/web/20230205235834/http://venturebeat.com/2016/02/24/yahoo-open-sources-caffeonspark-deep-learning-framework-for-hadoop/) 。甚至[谷歌也在某些项目上求助于 Caffe，比如 DeepDream](https://web.archive.org/web/20230205235834/http://googleresearch.blogspot.com/2015/07/deepdream-code-example-for-visualizing.html) 。

[Torch](https://web.archive.org/web/20230205235834/http://torch.ch/) 创建于 2002 年，由于其被脸书 AI Research (FAIR)使用，因此也很受欢迎。该公司在 2015 年初[开放了部分模块](https://web.archive.org/web/20230205235834/https://research.facebook.com/blog/fair-open-sources-deep-learning-modules-for-torch/)。其中一些工具经过优化，可在多台图形处理器或计算机上运行，以扩大容量并加快深度学习过程。同样，NVIDIA 的 cunn 是一个开源软件库，可以优化计算机的图形处理单元(GPU)性能，使机器学习更快。

这些工具虽然灵活且强大，但需要计算机视觉工程师和硬件团队，因此只有那些希望将计算机视觉作为其产品战略主要部分的公司(他们希望拥有该软件)才需要应用。

## 成衣:托管 API

不是每个公司都有资源，或者想投资资源，来建立一个计算机视觉工程团队。即使你找到了合适的团队，也可能需要做大量的工作才能让它恰到好处，这就是托管的 [API](https://web.archive.org/web/20230205235834/http://money.howstuffworks.com/business-communications/how-to-leverage-an-api-for-conferencing1.htm) 服务发挥作用的地方。这些解决方案在云中执行，提供开箱即用的图像识别服务菜单，可以轻松与现有应用程序集成，或用于构建特定功能或整个业务。

比如旅游频道需要“地标检测”，以便在特定地标的登录页面上显示相关照片，或者 eHarmony 希望过滤掉其用户上传的“不安全”的个人资料图片。这两家公司都不需要也不想进入深度学习图像识别开发业务，但仍然可以从其能力中受益。

[例如，谷歌云视觉](https://web.archive.org/web/20230205235834/https://cloud.google.com/vision/)提供一系列图像检测服务，从面部和光学字符识别(文本)到地标和露骨内容检测，并按每张照片收费。[微软认知服务](https://web.archive.org/web/20230205235834/https://www.microsoft.com/cognitive-services) (née [Project Oxford](https://web.archive.org/web/20230205235834/http://blogs.microsoft.com/next/2015/05/01/microsofts-project-oxford-helps-developers-build-more-intelligent-apps/#sm.00061tsqp117oer5v0v1y27ormftx) )提供了一系列视觉图像识别 API，包括情绪、名人和人脸检测，并对每 1000 笔交易收取特定的费用。与此同时，像 Clarifai 这样的初创公司提供计算机视觉 API，帮助公司组织他们的内容，过滤掉不安全的用户生成的图像和视频，并根据观看或拍摄的照片提出购买建议。

## 定制计算机视觉技术

当然，不一定是苹果或者橘子。计算机视觉工程团队不需要像谷歌一样大，不想建立自己的人工智能系统的大小公司可能仍然想要强大的定制图像识别解决方案。比方说，如果一家美容或化妆品公司想找到头发浓密的人的照片，为瘦身洗发水做广告，就需要有人创建一个定制算法来搜索头发浓密的人，因为这不是更商品化的解决方案提供的第一件事。

徽标或汽车品牌和型号也是如此，它们仍然是目前在开源领域不可用的利基商业应用程序。如果一个封闭的数据集不容易获得，也没关系，因为现在社交媒体上分享的图像有很大一部分是公开的，无论如何，这是一个丰富的图像来源，可以用来喂养机器学习野兽。

一些公司使用开放数据和开源框架的组合，只要他们有一个工程师团队，或者如果计算机视觉不是他们整个业务的赌注，他们可能只使用托管 API。

对于有各种非常特殊需求的公司，有定制的解决方案。然而，不管如何处理，很明显图像识别很少是孤立存在的；通过访问越来越多的图片、实时大数据、独特的应用程序和速度，它变得更加强大。充分利用这些联系的企业是最有可能取得成功的企业。