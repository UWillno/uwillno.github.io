# 本站Markdown多媒体语法说明
---
常规语法样式见[测试用例](?blog=test)，支持内部及查询参数路由，见[RSS](?rss)和[README#功能路由表](https://github.com/UWillno/uwillno.github.io/blob/main/README.md#%E5%8A%9F%E8%83%BD%E8%B7%AF%E7%94%B1%E8%A1%A8)，你可以自己查询参数内部跳自己文章，直接用我的md预览功能做一个纯Mardkwon博客。防剧透加密功能见[这篇文章](?blog=chlg5)。
这样基本上完全够用了。如果你在非我的网站看到这个文章，可能需要这样访问。[https://uwillno.com?func=mdeditor&source=https://uwillno.com/Markdown多媒体语法说明.md&preview](https://uwillno.com?func=mdeditor&source=https://uwillno.com/Markdown多媒体语法说明.md&preview)或者[https://uwillno.com?func=md&source=https://uwillno.com/Markdown多媒体语法说明.md](https://uwillno.com?func=md&source=https://uwillno.com/Markdown多媒体语法说明.md)
采用`md4c`解析，建议能用标准语法就不要扩展了，这样会导致其它markdown预览器无法正常解析。

`![]()`支持多媒体，仅通过后缀判断，暂时只写了几个主流后缀，在线链接需要允许资源跨域共享。
> 若有空格需要带上`<>`才可以被解析，这个标准语法并不是我扩展的。不支持带`|`的媒体文件。

## 表格

可以尝试表格中插入多媒体，至于效果和对齐是否正常不能保证。
表格面板去除了，可以通过长按来切换模式，因为难以确定你内容是否正常，“填满宽度”或“左右滑动”，左右滑动下换行需要依赖`<br/>`或`<br></br>`。对齐完全依赖Markdown语法。

## Latex支持

本质也算是图片，所以算作多媒体了。内联算表情高度默认为字体高度2倍，块级算图片高度为默认字体的4倍。所以块级Latex可以点开缩放。

## 图片
`![](https://iwmiu.dpdns.org/2024/04/07/profile/lzh1.jpg)`
![](https://iwmiu.dpdns.org/2024/04/07/profile/lzh1.jpg)
## 视频
> 不算稳定，技术预览中，慎用。
>> 浏览器中交互后才可以播放，通常播放时才能拿到视频尺寸，所以固定死，不提供任何扩展。

`![](https://github.uwillno.com/blogres/media/felgo.mp4)`
![](https://github.uwillno.com/blogres/media/felgo.mp4)

## 动图
`![动图样例](https://iwmiu.dpdns.org/2024/04/07/profile/test.gif)`
![动图样例](https://iwmiu.dpdns.org/2024/04/07/profile/test.gif)

## 音频
> 支持传入歌词和图片链接

`![](<https://github.uwillno.com/blogres/media/陈奕迅 - 于心有愧/陈奕迅 - 于心有愧.mp3|lrc=https://github.uwillno.com/blogres/media/陈奕迅 - 于心有愧/陈奕迅 - 于心有愧.lrc|cover=https://github.uwillno.com/blogres/media/cover/H3M.jpg>)`
![](<https://github.uwillno.com/blogres/media/陈奕迅 - 于心有愧/陈奕迅 - 于心有愧.mp3|lrc=https://github.uwillno.com/blogres/media/陈奕迅 - 于心有愧/陈奕迅 - 于心有愧.lrc|cover=https://github.uwillno.com/blogres/media/cover/H3M.jpg>)

## 图片扩展

`![](图片URL|[left|center|right]|pad|width=[数字|百分比]|pane)`

`[left|center|right]` 对齐方式
`pad` 图片不变换，除非尺寸很合理，不然不建议用。
`pane` 显示面板，背景和对齐按钮，表格中无效。
`width` 为百分比时宽度为 父控件的宽度*百分比。

> 移除height参数，通过宽度调节比较合理。
> 方便自行调整，已将图片控件还原至原始状态，默认`PreserveAspectFit`，`center`，不再启用面板。
>> 原始状态下，带鱼屏上如果不拆分可能看起来比较难受，通常这类md预览会大量两边留空或者拆分。

`![](https://44910244.xyz/%E5%88%98%E5%8F%AC%E8%BE%89/assets/image-20251106181303795.png|width=20%|center)`

![](https://44910244.xyz/%E5%88%98%E5%8F%AC%E8%BE%89/assets/image-20251106181303795.png|width=20%|center)

`![](https://44910244.xyz/%E5%88%98%E5%8F%AC%E8%BE%89/assets/image-20251106181303795.png|pane|pad|right)`
![](https://44910244.xyz/%E5%88%98%E5%8F%AC%E8%BE%89/assets/image-20251106181303795.png|pane|pad|right)


## 内联图片/表情
> 这算是常规语法，纯正则匹配来转为富文本<img>来显示，Qt默认文本控件就是这样显示图片的。

`:内部表情:`或`:img:链接|宽x高:` 可省略宽或高或`|宽x高`参数，
> 不支持百分比高宽，我认为不合理。

`:apl/smile:这是一段文本:img:https://44910244.xyz/%E5%88%98%E5%8F%AC%E8%BE%89/assets/image-20251106181303795.png|50x120:`
:apl/smile:这是一段文本:img:https://44910244.xyz/%E5%88%98%E5%8F%AC%E8%BE%89/assets/image-20251106181303795.png|50x120:

## 多媒体滑动视图
`![](["URL1","URL2"])`
> 注意链接要带双引号
`![](<["https://iwmiu.dpdns.org/2024/04/07/profile/lzh1.jpg","https://github.uwillno.com/blogres/media/felgo.mp4","https://iwmiu.dpdns.org/2024/04/07/profile/test.gif","https://github.uwillno.com/blogres/media/陈奕迅 - 于心有愧/陈奕迅 - 于心有愧.mp3|lrc=https://github.uwillno.com/blogres/media/陈奕迅 - 于心有愧/陈奕迅 - 于心有愧.lrc|cover=https://github.uwillno.com/blogres/media/cover/H3M.jpg","https://44910244.xyz/%E5%88%98%E5%8F%AC%E8%BE%89/assets/image-20251106181303795.png|pane|pad|left"]>)`
![](<["https://iwmiu.dpdns.org/2024/04/07/profile/lzh1.jpg","https://github.uwillno.com/blogres/media/felgo.mp4","https://iwmiu.dpdns.org/2024/04/07/profile/test.gif","https://github.uwillno.com/blogres/media/陈奕迅 - 于心有愧/陈奕迅 - 于心有愧.mp3|lrc=https://github.uwillno.com/blogres/media/陈奕迅 - 于心有愧/陈奕迅 - 于心有愧.lrc|cover=https://github.uwillno.com/blogres/media/cover/H3M.jpg","https://44910244.xyz/%E5%88%98%E5%8F%AC%E8%BE%89/assets/image-20251106181303795.png|pane|pad|left"]>)

有问题的话可能会调整。