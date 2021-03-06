# GetBingWallpaper
利用C#编写，Visual Studio 2015编译。将Bing首页的背景图下载并设置为系统桌面，程序默认为托盘形式，双击可唤出主要窗体。

[简化Python版](https://github.com/lxalxy/GetBingWallpaper/tree/py)

## 使用方法

打开程序后，右击托盘选择“Preview Today‘s Wallpaper"或双击托盘，会出现加载有今日壁纸的主窗体：

![](http://ww1.sinaimg.cn/large/6486a686ly1fclnnz056lj20m80ci7ot)

点击右上角√即可设置壁纸，点击×关闭窗体，鼠标放在i上可以获取该张壁纸的简单信息。

## 更新日志

### 2016.8.20

1. 利用Bing官方提供的XML格式API获取当日壁纸信息，下载并设置为桌面壁纸
2. 实现托盘运行

### 2017.1.28

1. 利用App.config文件进行设置的保存和读取
2. 可选是否保留历史壁纸，并自由设定保留天数和保存路径
3. 可选是否成功设置后自动退出
4. 可选开机自启

### 2017.1.29

1. 权限问题解决，参考[该链接](https://www.oschina.net/question/1041591_221434)，将启动信息写入当前用户注册表中

## To do

1. 各国有可能具有不同的每日壁纸，目前已实现了不同国家的API的获取，但壁纸不会更新，原因待查
2. 添加多屏不同分辨率支持

~~添加win10锁屏修改功能~~（除了UWP应用，微软貌似封掉了API）
