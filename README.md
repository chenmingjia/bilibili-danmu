# 项目说明
基于** Mask R-CNN**实现的视频蒙版弹幕，基本拥有bilibili官方的类似的效果。    
> 主要在后端提前根据原视频构建出人物的Mask， 本例子直接将视频和字幕合成，实际线上应该使用前端技术，将 mask 与 弹幕进行遮蔽。


# 视频效果截图

![image.png](https://upload-images.jianshu.io/upload_images/712028-62dabf5e29933bd8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/712028-79da82851c2a5721.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


# Requirements
- numpy
- tensorflow
- keras
- opencv
- [Mask R-CNN](https://github.com/matterport/Mask_RCNN)
- ... ...

# 准备工作

#### 1. 用 https://www.kanbilibili.com/ 来下载 B站视频和弹幕
例如：https://www.kanbilibili.com/video/av54944922?from=search&seid=13855581700550241007#download

#### 2. 然后用 DanmakuFactory_1.11_release 来将 xml 文件转化为 ass 字幕文件

#### 3. 使用格式工厂将视频和ass进行合成，产生原视频和字幕视频

#### 4. 下载 https://github.com/matterport/Mask_RCNN 源代码，在sample目录下运行该notebook

#### 5. 修改配置文件
