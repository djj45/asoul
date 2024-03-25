#### 软件下载

##### 带k轴的qq音乐歌词

###### github项目链接

https://github.com/MC-dusk/QRCD_M

###### 下载直链

https://github.com/MC-dusk/QRCD_M/releases/download/v0.2.1/qrcd_m_v0.2.1.7z

github项目链接有详细的使用方法，需要用到的歌词是og-char

##### aegisub的lua插件

###### github项目链接

https://github.com/qwe7989199/Lyric-Importer-for-Aegisub

###### 下载直链

https://github.com/qwe7989199/Lyric-Importer-for-Aegisub/archive/refs/heads/master.zip

根据对应的aegisub版本把文件放到aegisub对应的安装目录

##### 日语歌词自动注音软件

https://www.bilibili.com/video/BV11N411Q73v/

b站up主制作的软件，简介加群下载

#### 使用方法

1、用aegisub插件（安装好后插件在aegisub的自动化->Import Lyric File）导入og-char后缀的lrc歌词，用aegisub导出为ass歌词

2、把ass歌词放到b站up主的制作的`漢字注音辅助小工具（免费版）`，依次点击假名，转换，保存，把带注音的ass歌词导入aegisub

3、删除歌词自带的模板（如果有的话），在开头新建一行，把注释勾上，使用以下模板，然后应用卡拉ok模板即可

```
特效 template syl furi
内容 {\an5\pos($center,$middle)\K!$start/10!\K$skdur}

来源：https://home.gamer.com.tw/creationDetail.php?sn=3006854
```



