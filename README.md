A-SOUL录播，打轴，压制，投稿方法，请务必认真看完[介绍](#介绍)

全篇约1w5字，有图片，资料是自己收集的，感谢几位au私信评论区提供建议，用Typora写的markdown格式，有github版与gitee版，github与gitee同用户名同仓库名，可下载离线看，也可以在网页看（推荐）。Typora不能从一个文件传送到另外一个文件的某一个标题，gitee版在线观看效果最好，有大纲

方法包括b站和抖音录播，快速无损二刀流剪辑，提取直播唱的歌曲为mp3，aac/m4a格式，在直播过程中快速切出有歌词（中文，中日，中英等）的歌曲切片，简单的打轴和添加淡入淡出特效，弹幕压制，投稿等

有错误、问题、建议和补充欢迎评论区提出或者[b站私信我](https://space.bilibili.com/200257325/)

前后写了很长时间，到百度、谷歌、CSDN、维基百科、百度贴吧、b站、软件官网等网站找了很多资料，终于完结了，后续应该没有什么可以更新的了

#### 强烈推荐使用的软件

无损剪辑losslesscut，关键帧粗剪，不到3秒导出

https://github.djj45.workers.dev/mifi/lossless-cut/releases

#### TODO

FFmpegGUI，难者不会:hand:，期待大佬开发

目前有很多x264、ffmpeg或者其他编码器的GUI

https://github.djj45.workers.dev/zhen-ke/ffmpegGUI

https://github.djj45.workers.dev/hoshinohikari/StarTools

https://github.djj45.workers.dev/zyzsdy/NegativeEncoder

https://maruko.appinn.me/

https://gitee.com/haujet/QuickCut

https://ilharper.com/b/legacyproj#rmbox

但是我的想法是能有一款同时方便小白和懂音视频的人的软件，要跨平台，Mac和Windows都可以用，操作和参数可以自定义，这样不仅能随心所欲地调节自己想要的参数，还能作为其他命令行工具的GUI。软件一定要方便小白使用，把文件拖进去就ok了，无需多余的操作，不满足需求的人可以学习别人的参数或者导入配置，而大佬可以随意调节参数

比较符合我的想法的是

https://ilharper.com/b/legacyproj#rmbox

不过软件体积有点过于恐怖了，而且操作有点麻烦。我喜欢的界面是这个

https://github.djj45.workers.dev/zhen-ke/ffmpegGUI

#### 介绍

**视频教程（视频缓慢更新中，补充了一些文章里面没有提到的技巧，建议观看）**

https://www.bilibili.com/video/BV1mY4y1i7Ac

本文适合切片员和录播员，教你怎样录播切片加字幕投稿b站。这套方法入门可能需要不少时间，但是我保证绝对是视频成品质量最高，产出速度最快的方法。本文提到的所有软件都是免费、全平台的，除了剪映之外都是开源的。适用Windows与Mac（M1需要自行编译），原本所有程序的安装方法是Windows上的，现在增加了[在Mac上的使用方法](./mac.md)。可能会用到python，我写了[安装python的方法](./杂篇.md#python)

有疑问和建议欢迎私信，解决问题最快的办法就是私信我，有问必答：

https://space.bilibili.com/200257325

不建议使用的软件：

- 剪映，使用剪映识别字幕再用提取工具提取出来可以，把剪映用作字幕生成工具是没有问题的，但是剪映导出视频不能自定义音频码率，asoul的录播音频码率是320k，剪映只能导出128k的音频，音质效果不好
- arctime，arctime收费，没有必要付费，而且不付费功能不多，建议用开源免费的Aegisub
- 达芬奇windows版，导出aac格式的音频只能是128k，同剪映，mac版可以导出320k

在线流程图：

<img src="https://cdn.jsdelivr.net/gh/djj45/asoul@master/picture/asoul.svg" width=900 />

[离线流程图](./picture/asoul.svg)

新人快速入门：

[直播素材获取](./直播素材获取.md)+[字幕打轴](./字幕打轴.md)+[ffmpeg](./ffmpeg.md)+[b站投稿](./b站投稿.md)

- 用[分段下载工具](./直播素材获取.md#原画录播片段下载)下载自己想要切的片段
- 杂谈加字幕切片
  - 用[剪映专业版](https://lv.ulikecam.com/)语音识别生成字幕，再用[提取工具](./字幕打轴.md#自动生成字幕)提取出来，格式为srt
  - [下载安装自己喜欢的字体](./字幕打轴.md#字体)，把srt格式的字幕导入[Aegisub](./字幕打轴.md#下载)，[换成自己喜欢的字体样式](./字幕打轴.md#设置字幕样式)，字幕导出为ass格式
- 歌曲加字幕切片
  - [下载带有时间轴的srt字幕文件](./字幕打轴.md#LRC歌词)导入Aegisub，换成自己喜欢的字体样式，对准第一句的时间即可，字幕导出为ass格式
- [下载ffmpeg](./ffmpeg.md#ffmpeg下载及配置)并[配置环境变量](./ffmpeg.md#配置环境变量)，用[字幕压制命令](./ffmpeg.md#字幕压制)压制
- [核对视频](./ffmpeg.md#ffprobe的使用)后[投稿b站](./b站投稿.md)

如果想快速切片，必须自己[录播](./录播.md)

> Q:为什么用ffmpeg
>
> A:剪辑加字幕加弹幕当然可以用pr、达芬奇、剪映等软件，有图形界面，操作更简单，视频文章教程很多。但是我找不到系统介绍ffmpeg常用命令与原理的教程，所以查了很多资料自己总结了一份。ffmpeg跨平台，所有平台的命令都是一样的。ffmpeg对二刀流的视频进行加字幕、加弹幕、压制等处理非常高效，占用系统资源很小，非常适合用在Linux服务器上。ffmpeg命令接近音视频的原理，不同格式之间的转换非常简单快速，无损剪辑、视频无损转换、视频提取音频等功能其他软件难以替代。ffmpeg还可以录播，配合[抓流脚本](https://github.djj45.workers.dev/wbt5/real-url)可以录制很多平台的直播。ffmpeg处理多音轨多字幕的mkv格式电影很方便，不同语言的音轨和字幕提取出来，无损组成想要的电影。

#### [音视频知识](./音视频知识.md)

ffmpeg的基础，重点是封装格式，音视频格式，码率

#### [录播](./录播.md)

用b站录播姬或者blrec录播录弹幕

#### [直播素材获取](./直播素材获取.md)

网盘版的源码率录播与油猴插件下载b站视频，A-SOUL音乐素材获取，au制作的对二创有帮助网站，A-SOUL录音棚

#### [字幕打轴](./字幕打轴.md)

Aegisub的使用，找歌词，选字体

#### [FFmpeg](./ffmpeg.md)

压制转码，ffprobe，ffmpeg的使用，cmd命令行技巧

#### [Mac](./mac.md)

Mac用的人相对少，在Mac上录播和切片的教程估计没有，我虽然没用过mac，但是好在本文使用的软件都是开源的，在Mac上也可以使用

#### [b站投稿](./b站投稿.md)

转载与自制的区别，如何分区，加tag，分p

#### [杂篇](./杂篇.md)

PotPlayer配置，小丸工具箱下载和简单使用，dd烤肉机介绍，图片超分辨率，pr&ae教程，python的安装

#### [拓展阅读](./拓展阅读.md)

我写文章的时候参考的一些资料和知识拓展