---
title: 实惠app源码笔记
tag:
	- 日报
---

* * *

### 20161025
#### 大纲
1. 熟悉项目整体框架结构 ；
2. 熟悉项目AndroidManifest.xml文件；
3. 熟悉项目的gradle文件；
4. 熟悉项目的引用类库的作用；
5. 熟悉项目的自定义View的使用；
6. 熟悉项目360加固；
7. 熟悉项目的网络请求；
8. 熟悉项目的图片加载框架；
9. 熟悉项目的编码风格；
10. 其他；

#### 项目引用了5个library
* `androidgifdrawable`: 加载GIF图片库；**可选替代库：`Glide`；建议使用代码构建动画图片；**
* `swipemenu`：滑动菜单库;
* `roundedImageView`:圆形图片库；**可选替代库`//圆形图片 代码地址---->https://github.com/hdodenhof/CircleImageView`代替**
* `simplecropimagelib`：图片剪裁处理库；**可选替代库：**
* `pull_to_refresh_lib`:下拉刷新处理库；

#### 主项目`wemicommunity`
1. 网络请求底层使用httpClient请求；

##### 源代码功能很多地方使用了`JSONObject`和`JSONArray`解析json格式数据；
1. ShopCartFragment-》analysisStoreEntityList（）方法；

