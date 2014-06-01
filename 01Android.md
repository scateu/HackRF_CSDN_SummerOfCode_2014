
## 提案名称： 移植HackRF驱动到Android设备上

## 提案内容

**提案描述：**

HackRF是一款历史上首次从软件、固件、电路原理图和PCB板图完全开源而毫无保留的软件无线电平台，可以覆盖10MHz - 6GHz，已经在kickstarter上成功融资。将会使得更多的软件工程师、Linux黑客们获得直
接操作无线电波的可能。同时，对无线信号的安全分析也将会成为人们关注的新领域。

目前HackRF必须依赖于电脑才行工作，这给用户在外场进行使用带来了极大的不便。

Youtube上已经有人在一个Linux平板电脑上跑通了HackRF的驱动和gqrx程序。
同时，Android上也有人开发了[SDR Touch](https://play.google.com/store/apps/details?id=marto.androsdr2)等程序，证明了这个方案的可行性。

因此，我们的目标是在Android设备上使用USB On-the-go的方式将HackRF驱动起来

HackRF基于libusb库实现的USB设备驱动，提供libhackrf和hackrf-utils等源代码。

并且将基于Qt的gqrx程序移植到Android平板电脑上，打包成APK

具体要求:

1. 在安卓平台上移植libhackrf和hackrf-utils
2. 利用Qt的跨平台功能将gqrx移植到Android平台
3. 将libhackrf与gqrx进行对接，打包成为apk

**项目代码地址：**
 - <https://github.com/mossmann/hackrf>
 - <http://gqrx.dk/>
 - [SDR Touch](https://play.google.com/store/apps/details?id=marto.androsdr2)

**计划：**

* 中期检查前完成HackRF和gqrx和移植
* 结题之前完成APK的打包

**联系方式：**

* email: <cuckoohello@gmail.com>

## 对学生的要求

* 了解 Android 开发流程
* 了解 libusb 或一般USB驱动程序工作原理
* 对 Linux 上的一般程序编译/CMake/Makefile有了解

## 完成标准

 + hackrf_transfer程序运行之后不报错,OTG供电工作正常
 + APK打包后的gqrx可以直接在一般Android平台上运行
 + gqrx程序在20MHz采样率的工作状态下解调FM成功
