# Hosts Monitor 主机监控器

基于 glances 搭建的Linux集群监控。

### 技术栈

- 前端：vuejs+node应用 ： 单页面，模仿哪吒监控
- 后端：glances


哪吒监控-不支持容器监控
一个开源、轻量的服务器和网站监控、运维工具
https://nezha.wiki/
https://github.com/naiba/nezha

### Glances

glances 是一款用于 Linux、BSD 的开源命令行系统监视工具，它使用 Python 语言开发，能够监视 CPU、负载、内存、磁盘 I/O、网络流量、文件系统、系统温度等信息。
它还允许监控运行进程，登录用户，温度，电压，风扇速度等。它还支持容器监控，它支持不同的容器管理系统，如Docker，LXC。
信息显示在易于阅读的仪表板中，也可用于通过Web界面或命令行界面远程监控系统。它易于安装和使用，并且可以自定义为仅显示您感兴趣的信息。

官网
https://nicolargo.github.io/glances/
Github
https://github.com/nicolargo/glances
Docs
https://github.com/nicolargo/glances/wiki/
Docker
https://hub.docker.com/r/nicolargo/glances


glances 可以为 Unix 和 Linux 性能专家提供监视和分析性能数据的功能，其中包括：

- CPU 使用率
- 内存使用情况
- 内核统计信息和运行队列信息
- 磁盘 I/O 速度、传输和读 / 写比率
- 文件系统中的可用空间
- 磁盘适配器
- 网络 I/O 速度、传输和读 / 写比率
- 页面空间和页面速度
- 消耗资源最多的进程
- 计算机信息和系统资源

glances 工具可以在用户的终端上实时显示重要的系统信息，并动态地对其进行更新。
这个高效的工具可以工作于任何终端屏幕。
另外它并不会消耗大量的 CPU 资源，通常低于百分之二。
glances 在屏幕上对数据进行显示，并且每隔两秒钟对其进行更新。
您也可以自己将这个时间间隔更改为更长或更短的数值。
glances 工具还可以将相同的数据捕获到一个文件，便于以后对报告进行分析和绘制图形。
输出文件可以是电子表格的格式 (.csv) 或者 html 格式。

总结：python有瓶颈，下一个版本可能使用golang的监控作为核心。

### Glances Api

https://github.com/nicolargo/glances/wiki/The-Glances-RESTFULL-JSON-API

### 下版本计划

- 使用 ctop 替代 glances
ctop
https://github.com/bcicen/ctop