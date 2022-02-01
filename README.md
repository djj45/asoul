A-SOUL录播，打轴，压制，投稿方法，请务必认真看完[介绍](#介绍)

全篇约1w5字，有图片，资料是自己收集的，感谢几位au私信评论区提供建议，用Typora写的markdown格式，有github版与gitee版，github与gitee同用户名同仓库名，可下载离线看，也可以在网页看（推荐）。Typora不能从一个文件传送到另外一个文件的某一个标题，gitee版在线观看效果最好，有大纲

方法包括b站和抖音录播，快速无损二刀流剪辑，提取直播唱的歌曲为mp3，aac/m4a格式，在直播过程中快速切出有歌词（中文，中日，中英等）的歌曲切片，简单的打轴和添加淡入淡出特效，弹幕压制，投稿等

有错误、问题、建议和补充欢迎评论区提出或者[b站私信我](https://space.bilibili.com/200257325/)

#### 介绍

本文适合切片man，教你怎样切片加字幕投稿b站

新人快速入门：

[直播素材获取](./直播素材获取.md)+[字幕打轴](./字幕打轴.md)+[ffmpeg](./ffmpeg.md)+[b站投稿](./b站投稿.md)

- 用[直播素材获取](./直播素材获取.md)里面的分段下载工具下载自己想要切的片段
- 杂谈加字幕切片
  - 用[字幕打轴](./字幕打轴.md)里面的剪映语音识别生成字幕，再用提取工具提取出来，格式为srt
  - 下载安装自己喜欢的字体，把srt格式的字幕导入Aegisub，换成自己喜欢的字体样式，字幕导出为ass格式
- 歌曲加字幕切片
  - 下载带有时间轴的srt字幕文件导入Aegisub，换成自己喜欢的字体样式，对准第一句的时间即可，字幕导出为ass格式
- 下载ffmpeg并配置环境变量，用字幕压制命令压制
- 核对视频后投稿b站

如果想成为一位快速切片man，必须自己[录播](./录播.md)

#### [音视频知识](./音视频知识.md)

重点是封装格式，音视频格式，码率

#### [录播](./录播.md)

用b站录播姬录播录弹幕，用ffmpeg录播抖音

#### [字幕打轴](./字幕打轴.md)

Aegisub的使用，找歌词，选字体

#### [ffmpeg](./ffmpeg.md)

压制转码，ffprobe，ffmpeg的使用，cmd命令行技巧

#### [b站投稿](./b站投稿.md)

转载与自制的区别，如何分区，加tag，分p

#### [杂篇](./杂篇.md)

PotPlayer配置，小丸工具箱下载和简单使用，dd烤肉机介绍，图片超分辨率，pr&ae教程

#### [直播素材获取](./直播素材获取.md)

网盘版的源码率录播与油猴插件下载b站视频，A-SOUL音乐素材获取，au制作的对二创有帮助网站

#### TODO

- [ ] 硬件加速压制转码
- [ ] 不受自身网络影响的抖音录播软件（有blrec了，不过是仅仅针对b站的）