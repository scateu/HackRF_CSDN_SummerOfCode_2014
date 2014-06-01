
## 提案名称： 为HackRF提供一个网页版的解调前端

## 提案内容

**提案描述：**

HackRF是一款历史上首次从软件、固件、电路原理图和PCB板图完全开源而毫无保留的软件无线电平台，可以覆盖10MHz - 6GHz，已经在kickstarter上成功融资。将会使得更多的软件工程师、Linux黑客们获得直
接操作无线电波的可能。同时，对无线信号的安全分析也将会成为人们关注的新领域。

目前HackRF在计算机上的程序大部分是基于传统GUI程序提供的，例如gqrx基于Qt，SDRSharp基于C#。

我们现在想要实现一个基于浏览器/Javascript/Node.js的信号解调前端， 这样使用者在远程通过浏览器就可以直接对常见的信号进行观察，并能完成简单的WBFM NBFM AM解调的功能。

同时希望尽可能少的使用外部依赖库，尽可能优化其性能，使得能够在Raspberry Pi等嵌入式计算机上运行。这样用户就可以方便地部署天线架设更容易的场合。

具体要求:

1. 初步实现Node.js与libhackrf的集成
2. 在Node.js上初步实现FFT显示的功能
3. 使用Node.js实现瀑布图的功能
4. 基于Javascript实现FM/AM/SSB的解调功能
5. 优化网页前端，使得网页能够在iOS等移动设备的浏览器上正常运行
6. 在Raspberry Pi上优化性能
7. 发布代码,发布教程

**项目代码地址：**
<https://github.com/mossmann/hackrf>
<http://gqrx.dk/>
<http://websdr.org/>
<http://websdr.ewi.utwente.nl:8901/>
<https://github.com/kpreid/shinysdr>

**计划：**

* 中期检查前完成Node.js为后台的网页前端，实现FFT显示和瀑布图
* 结题之前完成FM/AM/SSB解调的功能，并实现在Raspberry Pi上部署

**联系方式：**

* email: <cuckoohello@gmail.com>


## 对学生的要求

* 熟悉 Javascript 开发
* 熟悉 Node.js 开发
* 基本了解FM解调的原理
* 在导师的指导下能理解 FFT 的基本思路，从而完成编码

## 完成标准

* 在常见浏览器上可以使用
* 可以正常观察信号的FFT和瀑布图
* 能够解调FM/AM/SSB信号
* 在Raspberry Pi上能够跑通
