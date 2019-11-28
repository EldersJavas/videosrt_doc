## video-srt

这是一个可以识别视频语音自动生成字幕SRT文件的开源`Windows-GUI`软件工具。

适用于快速、批量的为视频创建中/英文字幕文件的业务场景。

本项目使用了阿里云的[OSS对象存储](https://www.aliyun.com/product/oss?spm=5176.12825654.eofdhaal5.13.e9392c4aGfj5vj&aly_as=K11FcpO8)、[录音文件识别](https://ai.aliyun.com/nls/filetrans?spm=5176.12061031.1228726.1.47fe3cb43I34mn)的相关业务接口。

CLI（命令行）版本：[https://github.com/wxbool/video-srt](https://github.com/wxbool/video-srt)


## 界面预览
![界面预览](https://ae01.alicdn.com/kf/Hd5970633269141cc8c3341ab5397d714d.gif)


## Download 

##### 下载地址:(v0.1.2)
* .zip（含ffmpeg依赖） [点我下载](http://file.viggo.site/video-srt/0.1.2/video-srt-gui-ffmpeg-0.1.2-x64.zip)
* .zip（不含ffmpeg依赖） [点我下载](http://file.viggo.site/video-srt/0.1.2/video-srt-gui-0.1.2-x64.zip)

你也可以到 [release](https://github.com/wxbool/video-srt-windows/releases) 页面下载其他版本


## 注意事项
* 软件目录下的 `data`目录为数据存储目录，请勿删除。否则可能会导致配置丢失
* 项目使用了 [ffmpeg](http://ffmpeg.org/) 依赖，除非您的电脑已经安装了`ffmpeg`环境，否则请下载包含`ffmpeg`依赖的软件包


## FAQ
* 软件支持哪些语言？
    * 视频字幕文本识别的核心服务是由阿里云`录音文件识别`业务提供的接口进行的，设置好对应的语音引擎，可以支持汉语普通话、方言、欧美英语等语言
* 如何开通阿里云的相关服务？
    * 你需要有一个阿里云账号
    * 开通 `阿里云OSS对象存储` `阿里云智能语音交互` 业务
    * 在 `OSS对象存储` 控制台创建一个存储空间（Bucket）（读写权限设置为`公共读`）
    * 在 `智能语音交互` 控制台创建一个项目（根据使用场景选择识别语言以及偏好等）
    * 关于这块操作，后续会出一个视频教程，敬请关注。