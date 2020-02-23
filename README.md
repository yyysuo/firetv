**FireTV Stick 4K的特色**

- NetFlix和YouTube认证设备,原生客户端直接支持4K。最迷你, 最便宜的4K认证设备,对比Apple TV 4K的价格超便宜.  
- 比较开放，不需要刷机, 国内外播放软件通吃，随便安装。  
- 出差利器. 非常迷你,比遥控器还要小,可以隐藏在电视机后面.一个随身携带的专属播放器,在酒店随手插在电视上,连上wifi,国内外视频随意播放. 梯子客户端可以装在FireTV里,在外面的时候也可以自由播放NetFlix,YouTube.  

#### 开始前的准备工作

到手第一步，登录美亚帐户，并修改调试设置。

1）有美亚帐户直接登录，没有在美亚注册好了再登录。

2）进入FireTV系统设置。按遥控器Home键后，选Settings。

进入 Setting -> My FireTV-> Developer Options, ADB Debugging设置为ON，Apps from Unknown Sources 设置为ON。

返回后再进入 Setting -> My FireTV -> About -> Network，查看右侧 Fire TV 的IP Address（比如192.168.1.100）。记下来，后面会用到。

![](D:\BX02\Desktop\1912091125569b48e6edf12f0b.png)

#### 用电脑操作的教程

电脑上需要安装的软件: ADBLink 下载地址: [](http://www.jocala.com/)

1. 先下载如下2个apk在电脑上. （所有会用到的apk，都可以在本教程所在的页面找到)

    ATV_Launcher_0.1.5-pro.apk   
    FTVLaunchX-1.0.1.apk

2. 在电脑上运行ADBlink,输入前面准备工作中得到的FireTV IP，并点击连接。
   
   ![](D:\BX02\Desktop\TIM截图20200223200310.png)
   
   

3. 输入后你会在FireTV电视界面看到一个权限申请，点选总是允许，并确认。
   
   ![](D:\BX02\Desktop\200205113340977a864d567408.png)

4. 重新在电脑Adblink上面点击connect,这次已经能连上了。然后点击Install APK，把ATV_Launcher_0.1.5-pro.apk
   
    FTVLaunchX-1.0.1.apk
   
   安装在FireTV上面。
   
   

5. 在电脑Adblink上面点击Adb Shell,进入与FireTV的Adb调试界面。输入如下命令:
   
   ```
   pm grant de.codefaktor.ftvlaunchx android.permission.WRITE_SECURE_SETTINGS
   ```

6. 在FireTV上运行LaunchX，选择ATV Launcher为自己使用的桌面。设置好了以后，可以在ATV Launcher里面把LaunchX图标及Amazon自带的所有不用的程序图标全部隐藏起来。

7. 这样桌面替换就已完成。重复第4步，就可以安装其他常用的APP到FireTV上。
   
   

#### 用手机操作的教程

#### （需要安卓手机，没有的话，可以使用前面提到的电脑操作)

手机上需要预先安装的软件: （所有会用到的apk，都可以在本教程所在的页面找到)

![](D:\BX02\Desktop\19120911189f7f6674217b7a60.png)





1. 先下载如下3个apk在手机上. **只下载，不要安装在手机上.**

    ATV_Launcher_0.1.5-pro.apk  
    FTVLaunchX-1.0.1.apk

    remote-Adb.apk

2. 在手机上运行Apps2Fire,输入前面准备工作中得到的FireTV IP，并点击连接。

3. 输入后你会在FireTV电视界面看到一个权限申请，点选总是允许，并确认。

![](D:\BX02\Desktop\200205113340977a864d567408.png)

4. 用手机上的AppsFire把第1步下载的3个APK安装到FireTV上面，先不要在FireTV上运行。**如果安装APK到FireTV过程中失败, 把FireTV重启一下就可以了.**

5. 现在回到FireTV上面，运行刚刚安装的Adb Shell,进入与FireTV的Adb调试界面。(一般刚安装的APK会显示在桌面Home下面的Recent下。如果找不到的话, 进入 Setting, 再进Applications, 在里面找到后按菜单键,选择Launch,就可以运行了)
   
   a. 输入前面准备工作中得到的FireTV的IP，端口号为5555,然后connect.
   
   b. 输入后你会在电视界面再次看到一个权限申请，点选总是允许，并确认.
   
   c. 在提示符输入下面命令,不要有多余空格。

```
pm grant de.codefaktor.ftvlaunchx android.permission.WRITE_SECURE_SETTINGS
```

输入此条命令，有两种方式，一种是用遥控器一个字符一个字符的输入，还有一种方法，就是前面在手机上下载的Amazon FireTV这个软件连接盒子，在手机上复制，粘贴到盒子上面，简单方便不易出错.



6. 在FireTV上运行LaunchX，选择ATV Launcher为自己使用的桌面。设置好了以后，可以在ATV Launcher里面把LaunchX图标及Amazon自带的所有不用的程序图标全部隐藏起来。

7. 这样桌面替换就已完成。利用Apps2Fire就可以在手机上轻松安装其他常用的APP到FireTV上。
   
   
   
   #### 常用软件说明
   
   （所有提到的apk，都可以在本教程所在的页面找到)
   
   **a. 国外视频播放。**  
   
   1) NetFlix--- 从盒子提取的原生版本，供下载有困难的取用。  
   
    YouTube---从盒子提取的原生版本，供下载有困难的取用。  
   **b. 国内视频播放**  
   
   1) Perfect Player+自动更新播放源--- 直播国内外电视频道,强烈推荐。安装后,从顶部导航菜单齿轮状图标进去, 然后打开一般设置(General), 在播放列表1(Playlist1) 输入直播源地址:  
      [https://www.hefentv.cn/mtv/appgjh.m3u](https://www.hefentv.cn/mtv/appgjh.m3u) (2020年2月5号更新，此源已失效，自建源请看此帖  
      [https://www.hi-pda.com/forum/viewthread.php?tid=2676478](https://www.hi-pda.com/forum/viewthread.php?tid=2676478)  
      )
   
   