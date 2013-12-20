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

UI开发是Android开发的第一步工作。也是Android开发的基础。Android ui开发主要是基于View与ViewGroup。ViewGroup继承自View，但主要承担一个容器的角色。

### View ###
Android View 由边框和内容两部分组成，它们之间的距离成为padding。如下图：

![](/images/ui-develop/view-base-01.png)

View是所有显示类的基类，所有的widget(部件)都继承于它，所以掌握它的基本属性，对熟悉后面的组件有很大的帮助。

另外，Android提供了xml静态编写UI的方式，当程序运行的时候，会将整个layout.xml文件加载，实例化xml中所描述的View对象。这样的好处是：可以让我们更加快速的设计UI。同样我们也可以直接通过代码去实现UI。

在xml中所设定的属性，都会与Java类的方法一一对应，这个在DOC中都有详细的介绍。对于初学者，一定要明白xml中使用的这些属性，对应的方法是那些。因为这些属性有的是该View本身的属性，比如：id, background等；有的是其他类属性，如 layout_***，都是正对于布局时设定的属性。

事件处理


### ViewGroup ###

<!--more-->