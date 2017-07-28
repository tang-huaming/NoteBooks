# Ubuntu 16.04平台PJSIP环境搭建
首先，参考文章[VoIP应用在Ubuntu 14.04下编译FFmpeg libX264及PJSIP](http://blog.csdn.net/xiaohai911/article/details/40393205)完成基础的配置。

中间会需要用到一个NASM工具，Ubuntu默认提供的版本比较低，因此，需要自己到官网上面下载最新的版本并安装。

直到安装pjsip时，报错`alsa/asoundlib.h No such file`信息，需要安装一个音频库：

`apt install libasound2-dev`

但是，重新make仍然会出错，提示信息类似：`alsa_dev.c:(text+***) undefined reference to ***`

编译到这一步没法往下继续了，这时可以参照下面这篇文章按照默认的配置进行编译。

[Ubuntu下编译pjsip](https://segmentfault.com/a/1190000008338846)

这里提供了一种使用默认配置编译PJSIP的方法。
