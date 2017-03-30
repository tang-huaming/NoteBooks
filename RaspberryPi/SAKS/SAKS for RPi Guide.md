# 下载SDK
树莓派瑞士军刀扩展板SAKS SDK已经在github上开源，可以通过下面的命令下载：
> git clone https://github.com/spoonysonny/SAKS-SDK.git

下载完成后，进入根目录，可以查看该SDK的目录结构如下：

![SAKS SDK目录结构](http://i1.piimg.com/589674/ef9af54de96227db.png)

### 参考资料
- 【1】[树莓派瑞士军刀扩展板 SAKS SDK 发布](http://shumeipai.nxez.com/2015/09/21/saks-sdk-released.html)
- 【2】[树莓派瑞士军刀扩展板 SAKS SDK 升级](http://shumeipai.nxez.com/2016/06/10/saks-sdk-released-v2.html)
- 【2】[树莓派“瑞士军刀”扩展板（SAKS）DIY 教程](http://shumeipai.nxez.com/swiss-army-knife-shield-for-raspberry-pi-diy-tutorials)

# 配置环境
下载下来的SDK顶级目录名称为`SAKS-SDK`,我们可以将这个文件夹放置到任意位置，我将它放置到如下位置：

```
/home/pi/Documents/SAKS/sdk/SAKS-SDK
```

为了保证我们编写的Python代码能够找到这个SDK，我们需要在使用之前配置环境变量，将以上路径写入到`~/.profile`环境变量配置文件当中。使用vim打开`~/.profile`文件，在末尾添加如下代码：

```
export PYTHONPATH=$PYTHONPATH:/home/pi/Documents/SAKS/sdk/SAKS-SDK
```
保存并退出，然后执行如下命令：

```
source ~/.profile
```

至此，SAKS SDK的环境就已经配置完毕，你就可以使用Python的`import`命令导入相关的模块并使用了。