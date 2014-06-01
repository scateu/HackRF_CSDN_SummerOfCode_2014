
## 提案名称： 基于HackRF进行iBeacon协议分析

## 提案内容

**提案描述：**

GNURadio开源软件无线电框架提供了全面的对各种通信系统常用的信号处理模块，并提供了完整的信号开发模块，并已经形成完善良好的开源生态环境。但由于长久以来没有价格平易近人的硬件外设方案，使得GNURadio的学习门槛较高。HackRF的出现将使得开源软件无线电被大众普遍认识提供了可能。

HackRF是一款历史上首次从软件、固件、电路原理图和PCB板图完全开源而毫无保留的软件无线电平台，可以覆盖10MHz - 6GHz，已经在kickstarter上成功融资。将会使得更多的软件工程师、Linux黑客们获得直
接操作无线电波的可能。同时，对无线信号的安全分析也将会成为人们关注的新领域。

iBeacon是苹果公司2013年9月发布的移动设备用OS（iOS7）上配备的新功能。其工作方式是，配备有 低功耗蓝牙（BLE）通信功能的设备使用BLE技术向周围发送自己特有的ID，接收到该ID的应用软件会根据该ID采取一些行动。比如，在店铺里设置iBeacon通信模块的话，便可让iPhone和iPad上运行的应用软件将顾客进入店铺这一资讯告知服务器，或者由服务器向顾客发送折扣券及进店积分。此外，还可以在家电发生故障或停止工作时使用iBeacon向应用软件发送资讯，通知家电故障。

目前GNURadio已经提供了gr-bluetooth模块，可以供参考。

具体要求:

1. 使用已有的Bluetooth USB Dongle和iPad/iPhone跑通基本的iBeacon原理，写出教程
2. 跑通现有的gr-bluetooth模块
3. 基于现有的gr-bluetooth模块对iBeacon信号进行分析处理
4. 使用gr_modtool封装成为易于使用的工具集gr-ibeacon
5. 发布代码
6. 发布教程文章

**项目代码地址：**
<https://github.com/mossmann/hackrf>
<https://github.com/greatscottgadgets/gr-bluetooth>

**计划：**

* 中期检查前完成iBeacon信号原理的分析，能生成简单的iBeacon信号被苹果设备解析
* 结题之前完成gr-ibeacon模块的编写

**联系方式：**

* email: <putaoshu@gmail.com>


## 对学生的要求

* 能够在导师的指导下理解iBeacon/Bluetooth/GMSK
* 熟悉一般的 C++ 代码编写
* 对 Linux 下的软件开发有兴趣

## 完成标准

* gr-ibeacon模块可以发射iBeacon信号，被Apple设备解析
* gr-ibeacon模块可以接收由Apple设备发射的iBeacon信号，解析出传输的信息
