# Windows平台ARM裸机开发环境搭建
## 1 安装JVM

首先，你需要Java 8的JRE，下载地址如下：

[Java SE Development Kit 8 Downloads](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

## 2 下载Eclipse IDE for C/C++ Developers
可以直接去官网下载最新的版本，下面是地址链接：

[Eclipse IDE for C/C++ Developers](http://www.eclipse.org/downloads/packages/eclipse-ide-cc-developers/oxygenr)

![Markdown](http://i4.piimg.com/589674/490bb77f018b6601.png)

下载完成以后，直接解压，运行其中的`eclipse.exe`可执行文件，但是，这时会提示一个错误信息。这个主要是由于`eclipse.ini`配置文件设置错误引起的，需要做如下的改动：

![Markdown](http://i4.piimg.com/589674/e31fcf4fb6a2cec9.png)

修改配置文件中如上图所示的选中部分，保存并重新运行可执行文件，这时，你就可以看到程序可以成功启动了。

## 3 安装C/C++交叉编译器插件
启动Eclipse以后，依次选择`help -> Install New Software...`，会弹出安装插件的对话框。

下载GNU ARM工具链：[GNU ARM Embedded Toolchain](https://launchpad.net/gcc-arm-embedded)

> Eclipse开发环境搭建受阻，在[http://www.yagarto.org/](http://www.yagarto.org/)找到了两个推荐的IDE，可以用于ARM的裸机程序开发，测试一下。结果这里提供的两种方案都不行，都没有支持ARM11内核。

接下来，考虑转战Linux平台环境的搭建，或者是直接在虚拟机里面安装一个Windows XP，重新安装RVDS 2.2。
