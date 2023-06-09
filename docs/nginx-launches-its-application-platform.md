# Nginx 超越其服务器根基，推出其应用平台 

> 原文：<https://web.archive.org/web/https://techcrunch.com/2017/09/06/nginx-launches-its-application-platform/>

# Nginx 超越了它的服务器根，推出了它的应用程序平台

Nginx ，以其[商业](https://web.archive.org/web/20230209011150/https://www.nginx.com/)和[开源形式](https://web.archive.org/web/20230209011150/https://nginx.org/en/)，是当今互联网上最受欢迎的负载平衡器、代理、web 和应用服务器之一。但该项目的幕后公司 Nginx Inc .希望撒下更大的网，尤其是现在开发人员编写和部署他们的应用程序的方式正在迅速变化。正如该公司今天在波特兰举行的[开发者大会上宣布的那样，它将推出 Nginx 应用平台，为开发者提供一个一站式平台，用于开发或更新他们的应用程序，其中考虑了 DevOps、云、容器和微服务。](https://web.archive.org/web/20230209011150/https://www.nginx.com/nginxconf/?utm_source=nginxorg)

不出所料，该平台的核心是 Nginx Plus，该公司的商业版 Nginx 在开源版本的基础上增加了许多企业功能。除此之外，该公司还增加了 Nginx 控制器和 Nginx 单元。Controller 为应用程序(无论它们部署在哪里)提供了一个中央管理和控制平面，Unit 是一个现代应用服务器，用于运行在动态环境中的 PHP、Python 和 Go 编写的应用程序(支持 node.js、Java、Ruby Perl 和其他即将推出的应用程序)。今年晚些时候，单元将完全集成到控制器中，因此运营团队可以直接从控制器仪表板管理他们的单元应用程序。

“Unit 背后的想法是，例如，当代的应用服务器不太适合使用不同语言的微服务应用，”Nginx 产品负责人 Owen Garrett 告诉我。

该团队认为控制器是 Nginx Plus 和人们在其上运行的传统应用程序以及许多企业正在投资的现代绿色部署之间的桥梁。

控制器将于 10 月面向特定客户推出封闭测试版。单位已经可用。

现有的 Nginx Web 应用防火墙完善了该平台。整个平台的定价仍然悬而未决，而控制器仍处于封闭测试阶段。

同样值得注意的是，虽然 Unit 是开源的，但 Controller 是一个闭源项目。这遵循了 Nginx 保持其部分商业产品开源的长期传统。Nginx 首席技术官兼联合创始人伊戈尔·塞索耶夫告诉我:“我们希望 Unit 得到广泛采用，为此，我们需要开源它。”。"我们计划让控制器成为商业产品."该团队告诉我，他们希望尽快推出 Unit，以便从社区获得反馈，帮助他们决定该工具的未来方向。