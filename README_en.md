# uwillno.github.io / uwillno.com

## Languages

[🇨🇳 中文](README.md) | [🇬🇧 English](README_en.md)

## Introduce

- A static blog system developed based on Qt for WebAssembly, with some strange built-in functions
- For entertainment, technology attempts, learning and research, education for individuals, organizations, sand sculptures...
- The content includes but is not limited to individuals, organizations, sand sculptures, metaphysics, incorrectness, fiction... It is not recommended for those without the ability to discern.

## [Record page](https://uwillno.com/?blog)

### [Logs](https://uwillno.com/?blog)

Pure static, article (markdown, html)

![](assets/image-20250704142701094.png)

### [Moments](https://uwillno.com/?moment)

Edited short articles for internal use may be published at any time. Supports preview of all types of files and media.

![image-20250925163447838](assets/image-20250925163447838.png)

## [Function page](https://uwillno.com/?func)

Metaphysics-related functions are not ~~recommended~~ to use the true sun.

![image-20250704160229525](assets/image-20250704160229525.png)

### [Lunar Calendar](https://uwillno.com/?func=lunar)

[lunar](https://6tail.cn/calendar/api.html) call. It is not very compatible with Qt, there may be bugs, and the error message has been hidden.

![image-20250704160249404](assets/image-20250704160249404.png)

### [Six Yao](https://uwillno.com/?func=6yao)

Disk arrangement, direct migration of ancient versions is not guaranteed to be available.

![image-20250704160340431](assets/image-20250704160340431.png)

### [Xiao Liuren](https://uwillno.com?func=6ren)

![image-20250704173521223](assets/image-20250704173521223.png)

### [Huangji Jingshi](https://uwillno.com?func=hjjs)

According to the algorithm rewritten in the book, I compared it with the Tianji program. The results of the test cases are consistent. You can send me the abnormal use cases.

![image-20250704160442105](assets/image-20250704160442105.png)

![image-20250704173559129](assets/image-20250704173559129.png)

### [Tianji Notes](https://uwillno.com?func=tj)

The data source is unknown and has not been verified.

![image-20250704160502737](assets/image-20250704160502737.png)

![image-20250704173701749](assets/image-20250704173701749.png)

### [Ziwei Dou Shu](https://uwillno.com?func=zwds)

![image-20250925163256046](assets/image-20250925163256046.png)

### [Kaspersky Password Manager: txt to csv](https://uwillno.com?func=kpm)

### [Authenticator](https://uwillno.com?func=otp)

![image-20250704174008237](assets/image-20250704174008237.png)

### [QR code generation and recognition](https://uwillno.com?func=qr)

![image-20250704193108898](assets/image-20250704193108898.png)

### [WebSocket Test Tool/Chat Room](https://uwillno.com?func=ws)

The physical machine server starts irregularly

![image-20250704193221808](assets/image-20250704193221808.png)

### [Watermark Camera](https://uwillno.com?func=watermark)

Experiment only, it is recommended to use the Android version [QWMC](https://github.com/uwillno/qwmc_template)

![image-20250704193413779](assets/image-20250704193413779.png)

### [Image Stitching](https://uwillno.com?func=imagestitching)

![image-20250704193549478](assets/image-20250704193549478.png)

### [HTML editor](https://uwillno.com?func=htmleditor)

![image-20250704193648970](assets/image-20250704193648970.png)

### [Text Editor](https://uwillno.com?func=texteditor)

Modified from Qt official example [Qt Quick Controls - Text Editor | Qt Quick Controls](https://doc.qt.io/qt-6/qtquickcontrols-texteditor-example.html)

![image-20250704193708227](assets/image-20250704193708227.png)

### [AES](https://uwillno.com?func=aes)

![image-20250704193820710](assets/image-20250704193820710.png)

### [Personal Scheduling Query](https://uwillno.com?func=pb)

![image-20250704193840642](assets/image-20250704193840642.png)

![image-20250704193857546](assets/image-20250704193857546.png)

### [Periodic scheduling reasoning](https://uwillno.com?func=pba)

![image-20250704193957182](assets/image-20250704193957182.png)

### [Spine Viewer](https://uwillno.com/?func=spine)

![屏幕截图_2-11-2025_154634_cloudflare.uwillno.com](assets/屏幕截图_2-11-2025_154634_cloudflare.uwillno.com.jpeg)

![](assets/屏幕截图_2-11-2025_154712_cloudflare.uwillno.com.jpeg)

## [About page](https://uwillno.com?about)

Some content is not updated in a timely manner because the developers are particularly lazy.

![image-20250704192548096](assets/image-20250704192548096.png)

### [This program](https://uwillno.com?about=program)

![image-20250704192623476](assets/image-20250704192623476.png)

### [History of this site/Message](https://uwillno.com?about=website)

![image-20250704192526733](assets/image-20250704192526733.png)

### [Me](https://uwillno.com?about=me)

![image-20250704192658563](assets/image-20250704192658563.png)

## [Link page](https://uwillno.com?links)

![image-20250925163127610](assets/image-20250925163127610.png)

## Other

### [RSS](https://uwillno.com?rss)

### Settings (particle system, effects, language, theme, frame rate display, background switching, music player switch)

![image-20250704194050755](assets/image-20250704194050755.png)

![image-20250925163602110](assets/image-20250925163602110.png)

![](assets/image-20251102155606040.png)

### Light/dark mode

### Music player

![image-20250704194157886](assets/image-20250704194157886.png)

### Vertical screen

![image-20250704194447724](assets/image-20250704194447724.png)

### Horizontal screen

![image-20250704194540493](assets/image-20250704194540493.png)

### ……

## Note

- The .wasm file is relatively large, so pay attention to traffic consumption. Some areas require proxy access.
- Many BUGs are in the Qt framework itself. Some modules are in the technology preview stage. Occasionally, upgrading the Qt version will cause instability.
- Even if we can locate the problem, we will not modify the Qt source code itself, but will prioritize finding and adopting coding avoidance solutions.
- Coding habits and development ideas are too weird, with almost no usability to third parties, mixed with private files, and no complete source code is provided
- After ~~2.0, it will be changed to single-threaded construction. The execution efficiency of complex operations may be reduced. Decoupling will be carried out, and functions will be gradually added back as needed~~
- Compatibility with Android WebView has been abandoned and multi-threaded construction is used to improve operating efficiency.

## Reference

<hr/>

- [Qt](https://www.qt.io/)
- [emscripten](https://emscripten.org/)
- [Cloudflare](https://www.cloudflare.com/)
- [Github](https://github.com/)
- [coi-serviceworker](https://github.com/gzuidhof/coi-serviceworker)
- [Gravatar](https://gravatar.com/)
- [Qt-AES](https://github.com/bricke/Qt-AES/)
- [Lunar](https://6tail.cn/calendar/api.html)
- [DBWnl](https://github.com/jkinfeng/DBWnl)
- [fontello](https://fontello.com/)
- [iconfont](https://www.iconfont.cn/)
- [MiSans](https://hyperos.mi.com/font/zh/)
- [Kaspersky](https://www.kaspersky.com)
- [Azur Lane](https://game.bilibili.com/blhx/)
- [Esterv.Utils.QrCode](https://github.com/EddyTheCo/Esterv.Utils.QrCode)
- ……
- Including but not limited to the above content, which may no longer exist in the current version, but has been used or referenced.

## Historical version

Originally they were all kept in the warehouse. Recently, the warehouse size was reduced and removed. Here is a screenshot to commemorate.

### widgets version

When I was in college, I tried to write Qt for webassembly randomly, and only had a few functions for my own use.![old](assets/old.jpeg)

### 1.0.5Preview

Re-developed based on Qt Quick and built with multi-threading. In the later period, it was too confusing and difficult to maintain, so it was rebuilt.

![1.0.5](assets/1.0.5.jpeg)

## Notice

All documents, including this article, are machine translated and accuracy cannot be guaranteed!
