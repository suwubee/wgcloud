<p align="center">
  <a  target="_blank" href="http://www.wgstart.com">
    <img src="./demo/logo.png">
  </a>
 </p>



## WGCLOUD介绍

WGCLOUD设计思想为新一代极简运维监控系统，提倡快速安装，降低运维学习成本，全自动化运行，无模板和脚本。当前仓库版本为v2.3.6。

WGCLOUD基于轻量级springboot架构，是高性能高并发的分布式监控系统，核心模块包括：**主机监控，ES集群管理，CPU监控，CPU温度监控，大屏可视化展板，内存监控，数据监控(mysql，oracle，pg等)，服务心跳检测，应用进程管理，磁盘空间和IO监控，硬盘smart健康检测，系统负载监控，网络拓扑图，端口监控，日志文件监控，docker监控，Web版SSH，堡垒机，监控告警信息（可集成微信钉钉短信等方式）推送**。[english readme](<./README_en.md>)

1.采用服务端和客户端协同工作方式，更轻量，更高效，后可支持5000+台主机同时在线监控。

2.server端负责接受数据，处理数据，生成图表展示。agent端默认每隔30秒(时间可调)上报指标数据。

3.支持主流服务器平台安装部署，如Linux, Windows,macOS, Solaris, AIX, HP-UX等。

4.WGCLOUD采用springboot+bootstrap，完美实现了分布式监控系统，为反哺开源社区，二次开源。

5.v2即当前仓库为开源版，**v3为商业版（分免费个人版和付费专业版）**，商业版功能更多，性能更优秀，请点击查看[开源版和商业版区别](<./开源版和商业版区别.md>)

6.如果你觉得WGCLOUD帮助到了你，请移步网站打赏支持下，感谢

## **网站**

<http://www.wgstart.com>

## **演示**

打开<http://www.wgstart.com>后，在网站顶部点击【演示】链接即可，免密登录

## **视频**

B站WGCLOUD相关视频地址，<https://space.bilibili.com/549621501/video>

## **源码使用**

1.使用IDEA的话（推荐），直接打开wgcloud-server和wgcloud-agent即可，JDK使用1.8

2.使用Eclipse的话，导入maven工程wgcloud-server和wgcloud-agent即可，JDK使用1.8

2.运行所需sql脚本（本项目使用mysql数据库），在sql文件夹下，在mysql数据库里创建数据库wgcloud，导入wgcloud.sql即可

3.wgcloud-agent运行所需sigar的so，dll等文件，在sigarLibs里，解压后可用，开发环境注意配置编译器的VM参数即sigarLibs路径：-Djava.library.path=E:\wgcloud-agent-v2.3\sigarLibs

## **功能截图**



![WGCLOUD监控主面板](./demo/demo2.jpg)

![WGCLOUD监控主机列表](./demo/demo3.jpg)

![WGCLOUD监控主机列表](./demo/daping.jpg)

![WGCLOUD监控图表](./demo/demo4.jpg)



![WGCLOUD网络拓扑图](./demo/tpdemo.jpg)

![WGCLOUD主机web ssh客户端图](./demo/ssh.jpg)

![WGCLOUD主机画像图](./demo/huaxiang.jpg)


## 运行环境

1.JDK1.8

2.mysql5.6 或 5.7

3.跨平台，linux：内核版本2.6.23或更高，CentOS/RHEL 6.0以上。windows：windows server 2003以上

## 联系

邮箱：tianshiyeben@qq.com

## 感谢

JetBrains提供的免费license