# Bitnami 的新 Stacksmith 服务让开发者更容易构建定制应用容器 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2015/11/16/bitnamis-new-stacksmith-service-makes-it-easier-for-developer-to-build-custom-app-containers/>

Bitnami 最出名的可能是只需点击几下鼠标就能轻松部署网络应用、服务和开发环境。随着开发人员开始转向容器，Bitnami 也必须改变以跟上这一趋势。该公司今天在巴塞罗那的 Docker 开发者大会上发布了 Stacksmith 的第一个测试版。

Stacksmith 为开发人员提供了一套“高质量、更新和管理的应用程序组件”,他们可以在 Docker 中用于开发和生产。Bitnami 表示，这项服务建立在现有的一套管理运行时和组件的基础上，并将高级应用程序需求转化为 Docker 文件。

“通过向这个 Docker 文件添加应用程序代码，应用程序及其所有依赖项都被捕获到一个易于共享、可定制的 Docker 文件和容器映像中，该映像适合现有的构建和部署工具，”该公司解释了其新服务。Bitnami 指出，例如，开发人员可以选择 Python、Java、PHP、Go、Ruby 或 Node 等语言，以及他们喜欢的这些语言的框架来构建他们的容器化开发环境。

构建这些客户容器图像应该只需要几分钟，一旦它们可用，开发人员也可以通过一个 URL 轻松地共享它们。

“通过使用 Stacksmith 服务，应用程序开发人员可以将自己从对框架依赖性和低级 Linux 需求的担忧中解放出来；Bitnami 产品副总裁 Simon Bennett 在今天的声明中说:“他们可以专注于使用他们选择的语言来开发优秀的软件。“这个测试版的目标是我们希望社区建立尽可能多的不同类型的图像，并以一种我们从未预料到的方式使用 Stacksmith 。我们喜欢惊喜。”

为了确保这些新容器的安全性，Bitnami 将在这些自定义容器中的组件出现安全问题或其他更新时通知开发者。

除了 Stacksmith 之外——基于它——Bitnami 今天还宣布在 Google 的容器注册表中发布一组用于公共语言运行时的新容器映像。

“我们希望让容器的开发变得简单，Bitnami 的新stack Smith服务是朝着这个方向迈出的一大步，”谷歌负责谷歌容器注册的产品经理 Kit Merker 说。“Google Container Registry 是一种快速、安全且经济高效的存储容器的方式。这两种服务的结合让您可以声明从可重复使用的基础映像生成 Docker 文件的依赖关系。”

谷歌和 Bitnami 最近似乎关系不错。例如，两家公司之前曾合作将 Bitnami 应用程序引入谷歌云平台。在那里，焦点也是让开发者在谷歌的服务器上建立有管理的开发者环境变得容易。