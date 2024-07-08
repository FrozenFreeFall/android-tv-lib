

# Android_tv_libs
android tv 相关的库，包括界面开发，播放器等等的收集，

我并无法保证全部加入，必定会遗漏一些优秀的TV相关的库，

欢迎大家一起往里面添砖加瓦.



TV开发 QQ群1：522186932(人满) QQ群2:468357191(已满) QQ群3:976338508

android tv交流网站: www.androidtvdev.com

android tv文章专题：https://www.jianshu.com/c/3f0ab61a1322

已回海南乐东老家休息，可接 Android TV 相关的UI项目.

[TOC]


# 一. 控件



## Leanback相关：

### 1.谷歌 leanback demo

项目地址：https://github.com/googlesamples/leanback-showcase

谷歌原生的 leanback demo，看完此demo，基本就懂如何使用了.

leanback很灵活，主要是MVP的思想.

![](https://github.com/googlesamples/leanback-showcase/raw/master/screenshots/Showcase-Snapshots.png)



### 2.V14Leanback 

项目地址：https://github.com/DukerSunny/V14Leanback

该项目主要是将leanback代码复制出来了.

一个适用于Android TV端的分页加载列表库，控件继承自RecyclerView，部分源码抽取自Google Support v17 Leanback包下源码，可兼容低版本环境。



### 3.Leanback修改代码

项目地址：https://github.com/FrozenFreeFall/Leanback_tv_widget

项目只修改了一些代码.

![](https://camo.githubusercontent.com/b91bdf3ae32ea2946930e96e54d5198f5ad4552a/687474703a2f2f6769742e6f736368696e612e6e65742f75706c6f6164732f696d616765732f323031362f313233302f3133333531355f32613364663236365f3131313930322e706e67)


### 5. BrowseFragment 自定义

项目地址：https://github.com/dextorer/Sofa

A library for Android TV that extends the Leanback library functionalities

对 Leanback 库的BrowseFragment 进行自定义，让一个 Header对应一个页面。不过最新 Leanback 库已经支持该功能。

![](https://images.gitee.com/uploads/images/2019/0522/165936_87fdc511_111902.jpeg)



### 4.TwoWayView

项目地址：https://github.com/lucasr/twoway-view

此项目可以配合leanback使用，嵌入1 N 布局，需要修改leanback源码.

![](https://images.gitee.com/uploads/images/2019/0522/165931_a66cb1ec_111902.png)

## RecyclerView相关：



### 1. CustomTvRecyclerView 

项目地址：https://github.com/songwenju/CustomTvRecyclerView

该项目实现了 RecyclerView 按键翻页效果，可以参考代码并使用.

![](https://github.com/songwenju/CustomTvRecyclerView/raw/master/raw/master/screenshots/tvRecycler2.0.gif)



### 2. TVRecyclerView

项目地址：https://github.com/Fredlxy/TVRecyclerView

封装过的RecyclerView，用于TV开发，



### 3. TvRecyclerView--针对TV端特性进行的适配与开发

项目地址：https://github.com/zhousuqiang/TvRecyclerView

此项目在TwoWayView的基础上进行的改进，支持焦点快速移动，支持Item选中放大时不被叠压(无需手动调用bringChildToFront())，支持横/竖排列，支持设置选中Item边缘距离/居中，支持设置横竖间距，Item监听回调

![](https://github.com/zhousuqiang/TvRecyclerView/raw/master/images/img_all.gif)


### 4. TvRecyclerView

项目地址：https://github.com/henryblue/TvRecyclerView 

用在android TV端的自定义recyclerView控件, 不支持手机端.

![](https://images.gitee.com/uploads/images/2019/0522/165933_1357ab48_111902.png)


### 4. VLayout

项目地址：https://github.com/FrozenFreeFall/vlayout

这么说的，虽然只是移动端，并不支持TV端，但是此控件的思想不错，也避免了leanback在低配机器耗性能的问题(Recyclerview嵌套)，修改支持TV端，是一个神器.

![](https://camo.githubusercontent.com/2b947a15f5502af5a4639a5927d68052ccfb54a3/687474703a2f2f696d67332e746263646e2e636e2f4c312f3436312f312f31623962666234323030393034376637356365653038616537343135303564653263373461633061)

### 5. tangram

项目地址：https://github.com/alibaba/tangram-android

项目相关文章：https://mp.weixin.qq.com/s/S1yP_RSgDfqFSbuDImrpuw

使用JSON的数据格式来加载界面，很有参考和学习的代码.



## 适配库：



### 1. AutoLayout

项目地址：https://github.com/hongyangAndroid/AndroidAutoLayout

文章: https://blog.csdn.net/lmj623565791/article/details/49990941

作者暂时不维护了，为了支持没有的控件或者未知函数，需要改一些东西.

使用的很简单，添加设计图分辨率，使用PX... ...



### 2.SupportMultipleScreensUtil

项目地址：https://github.com/baixiaoY/SupportMultipleScreensUtil

调用方便，只需要调用它的转换函数就OK了.

### 3. AutoUtils

项目地址: https://gitee.com/kumei/android-tv-frame-new/blob/develop/AndroidTvWidget/tvlib/src/main/java/com/open/tv/common/AutoUtils.java

手动写适配，简单易用


### 4.工具生成values

工具地址：https://gitee.com/kumei/AndroidTVWidget/tree/master/Tool

这种方式不建议使用了，新出的机型分辨率需要重新生成，pass吧.

### 4.ConstraintLayout

Android新出的约束，也可以用于部分适配，还是不错，也能优化界面的布局，避免嵌套太深.



## TV框架：

###1. Android tv metro

项目地址：https://gitee.com/kumei/android_tv_metro

此项目由开源社区修改，可编译版本，并添加了代码分析注释，原始源码自行下载.

在此重点说明下：tv metro的架构思想和部分代码是很有参考价值的，布局是动态生成的.



### 2. Android tv frame

项目地址：https://gitee.com/kumei/AndroidTVWidget

最新项目重构地址：https://gitee.com/kumei/android-tv-frame-new

此项目包含了 移动边框，键盘，listview, gridview, recylerview等等

![](http://git.oschina.net/uploads/images/2016/0406/110716_e9f61513_111902.png)



### 3. tv widget

项目地址：https://github.com/evilbinary/TvWidget

此项目可以库使用，也可以作为代码学习，还是不错.

![](https://images.gitee.com/uploads/images/2019/0601/005424_84694f54_111902.png)



### 3.移动边框BorderViewDemo

项目地址：https://github.com/lf8289/BorderViewDemo



## Launcher源码：

### 1. SMTVLauncher

项目地址：https://github.com/FrozenFreeFall/SMTVLauncher

![](https://images.gitee.com/uploads/images/2019/0601/005424_0fdce2ec_111902.jpeg)



### 2. AndroidTVLauncher

项目地址：https://github.com/JackyAndroid/AndroidTVLauncher

此项目基于 Leanback，可以参考参考别人使用leanback的代码.

![](https://github.com/JackyAndroid/AndroidTVLauncher/raw/master/screenshots/design_sketch1.png)


### 3. TVSample

项目地址：https://github.com/hejunlin2013/TVSample

两个 TV Launcher 页面例子：

1、仿泰捷视频最新TV版 Metro UI。

2.仿腾讯视频 TV 版(云视听·极光) 列表页(用 RecycleView + GridLayoutManager 实现)

![](https://github.com/hejunlin2013/TVSample/raw/master/images/device-2016-10-13-191954.png）


### 4. Leanback桌面demo

项目地址: https://gitee.com/chuangshiji/Launcher


## 动画库:

### SVG动画

项目地址: https://github.com/alexjlockwood/adp-delightful-details

![](https://images.gitee.com/uploads/images/2019/0601/005439_050a807c_111902.gif)

项目地址：https://github.com/Pixplicity/sharp



### recyclerview-animators 动画库

项目地址: https://github.com/wasabeef/recyclerview-animators


### 转场动画

项目地址: https://github.com/lgvalle/Material-Animations



## 其它View相关：



### 1.阴影控件 

项目地址：https://github.com/yingLanNull/ShadowImageView

![](https://images.gitee.com/uploads/images/2019/0601/005434_288a4a3b_111902.png)

### 2.角标控件

项目地址: https://github.com/H07000223/FlycoLabelView，https://github.com/linger1216/labelview

![](http://git.oschina.net/uploads/images/2016/0301/115509_4dfe34ba_111902.png)


### 3. 圆角控件

项目地址: https://github.com/Y-bao/RoundAngleFrameLayout

![输入图片说明](https://images.gitee.com/uploads/images/2018/1031/002556_4cbe9ff8_111902.png "圆角控件")

### 4. 星级控件

项目地址: https://github.com/DreaminginCodeZH/MaterialRatingBar

![](https://images.gitee.com/uploads/images/2018/1101/162250_0ba661bb_111902.png "")

# 二. 播放器



### 1.UPYUN Android 流媒体播放器

项目地址:https://github.com/upyun/android-player-sdk

android-player-sdk 是一个适用于 Android 平台的影音播发器 SDK ，基于 ijkplayer ( based on ffplay )，可高速定制化和二次开发，为 Android 开发者提供简单，快捷的接口。

### 2.GSYVideoPlayer

项目地址：https://github.com/CarGuo/GSYVideoPlayer

视频播放器（IJKplayer），HTTPS支持，支持弹幕，支持滤镜、水印、gif截图，片头广告、中间广告，多个同时播放，支持基本的拖动，声音、亮度调节，支持边播边缓存，支持视频本身自带rotation的旋转（90,270之类），重力旋转与手动旋转的同步支持，支持列表播放 ，直接添加控件为封面，列表全屏动画，视频加载速度，列表小窗口支持拖动，5.0的过场效果，调整比例，多分辨率切换，支持切换播放器，进度条小窗口预览，其他一些小动画效果，rtsp、concat、mpeg。简书:<http://www.jianshu.com/p/9fe377dd9750>

![](https://github.com/CarGuo/GSYVideoPlayer/raw/master/33.gif)


### 3.ExoPlayer

项目地址：https://github.com/google/ExoPlayer/


# 三. TV输入法

### 1. 原生的谷歌输入法，可单独编译版本.

项目地址:https://gitee.com/kumei/PinyinIME_GOOGLE 

### 2. 英文输入法.高仿搜狗界面.

项目地址:https://gitee.com/kumei/OpenInputMethod 



# 四. 其它



### 1. 反射库

项目地址：https://github.com/jOOQ/jOOR

很方便的使用反射函数，简单，高效，一行代码搞定反射调用，不用写很多代码



### 2.进程间通信库Hermes

项目地址：https://github.com/Xiaofei-it/Hermes-IPC-Demo

项目地址：https://github.com/Xiaofei-it/Hermes

项目地址：https://github.com/elemers/HermesEventBus 跨进程通信的eventbus


### 3.基于JSON RPC的一种Android跨进程调用

文章解读：https://www.jianshu.com/p/1eca5e32fad2?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io

项目地址：https://github.com/iqiyi/Andromeda


### 4. 权限管理SDK

项目地址:https://github.com/yanzhenjie/AndPermission

官方网站:http://yanzhenjie.github.io/AndPermission/cn


# 五. 工具


阴影生成工具: https://inloop.github.io/shadow4android/


# 六. 网络相关

### 1. 远程控制你的智能电视，按键|输入|安装App等都已实现.

项目地址：https://github.com/NanoHttpd/nanohttpd

文章地址：https://juejin.im/post/5a9e47636fb9a028c42db81d


### 2. OkGo，一个专注于让网络请求更简单的框架，与RxJava完美结合，比Retrofit更简单易用。

项目地址：https://github.com/jeasonlzy/okhttp-OkGo

文章地址：https://www.jianshu.com/p/6aa5cb272514
ta 
