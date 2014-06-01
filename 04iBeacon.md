
## 提案名称： 基于HackRF进行iBeacon协议分析

## 提案内容

**提案描述：**

GNURadio开源软件无线电框架提供了全面的对各种通信系统常用的信号处理模块，并提供了完整的信号开发模块，并已经形成完善良好的开源生态环境。但由于长久以来没有价格平易近人的硬件外设方案，使得GNURadio的学习门槛较高。HackRF的出现将使得开源软件无线电被大众普遍认识提供了可能。

HackRF是一款历史上首次从软件、固件、电路原理图和PCB板图完全开源而毫无保留的软件无线电平台，可以覆盖10MHz - 6GHz，已经在kickstarter上成功融资。将会使得更多的软件工程师、Linux黑客们获得直
接操作无线电波的可能。同时，对无线信号的安全分析也将会成为人们关注的新领域。

iBeacon是Apple公司主推的新一代近场通信的协议，主要基于低功耗的蓝牙4.0技术。
目前GNURadio已经提供了gr-bluetooth模块

具体要求:

1. 使用已有的Bluetooth USB Dongle和iPad/iPhone跑通基本的iBeacon原理，写出教程
2. 跑通现有的gr-bluetooth模块
3. 基于现有的gr-bluetooth模块对iBeacon信号进行分析处理
4. 封装成为易于使用的工具集
5. 发布代码及教程文章

**项目代码地址：**
<https://github.com/mossmann/hackrf>


**其他需求：**
* 编码遵循Ruby语法规范
* 前端遵循现有框架，新增页面风格需跟现有页面保持一致

**计划：**

* 中期检查前完成Fork 功能
* 结题之前完成Pull Request 功能

**联系方式：**

* email: <putaoshu@gmail.com>


## 对学生的要求

* 熟悉 Android 开发
* 熟悉 libusb 的工作原理

## 完成标准

* Fork完成标准：
	+ 完成90％以上的功能要求
	+ 有单元测试，覆盖率 > 50%
* Pull Request完成标准
	+ 完成70％以上的功能要求
	+ 有单元测试，覆盖率 > 50%
