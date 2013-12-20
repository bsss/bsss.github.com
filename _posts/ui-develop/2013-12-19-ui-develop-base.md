---
title: Android UI开发基础
author: yanjun
layout: post
category : Android UI
permalink:  /ui-develop-base/
tags: 
  - Android
  - UI
  
---

UI开发是Android开发的第一步工作。也是Android开发的基础。Android ui开发主要是基于View与ViewGroup。ViewGroup继承自View，但主要承担一个容器的角色。它们共同组成了View树。

<!--more-->

![](/images/ui-develop/view-base-01.png)

Android UI可以直接使用代码编写，同时也提供了xml静态编写UI的方式，当程序运行的时候，会将整个布局文件加载，实例化xml中所描述的View对象。这样可以让我们更加快速的设计UI。

## View ##
Android View 是用一个矩形来描述的，由边框和内容两部分组成，它们之间的距离称为padding。如下图：

![](/images/ui-develop/view-base-02.png)

View是所有显示类的基类，所有的widget(部件)都继承于它，所以掌握它的基本属性，对熟悉后面的组件有很大的帮助。

通过静态方式设计UI时，xml中所设定的属性，其实都会与相应Java类的方法一一对应，在DOC中都有详细的介绍。对于初学者，一定要明白xml中所使用的这些属性，对应的方法是那个。这些属性有的是该View本身的属性，比如：id, background等；有的是其他类属性，如 layout_***，都是针对于布局参数设定的属性。

### View 常见属性 ###

事件处理


## ViewGroup ##

