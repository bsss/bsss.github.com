---
title: Ubuntu下搭建NDK环境
author: JinMa
layout: post
category : Android
permalink:  /ndk-environment-to-build/
tags: 
  - Android
---
##**Ubuntu下搭建NDK环境**
####第1步：
下载文件：android-ndk-r8c-linux-x86.tar.bz2</br>
[gitBub下载][1]</br>
解压后得到一个文件夹android-ndk-r7</br>
<!--more-->
tar -xjf android-ndk-r8c-linux-x86.tar.bz2</br>

####第2步：
(终端下)#vi .bashrc，在最后加上如下一行</br>
export PATH=$PATH:/home/user/android-ndk-r57</br>
保存，退出
####第3步：
使得刚刚的设置生效
source .bashrc

####第4步：
测试环境是否配置成功</br>
cd android-ndk-r7 </br>
cd sample/hello-jni/jni </br>
ndk-build </br>

这样就会出现如下提示信息，证明成功，同时出现lib和obj两个文件夹

    Gdbserver      : [arm-linux-androideabi-4.4.3] libs/armeabi/gdbserver
    Gdbsetup       : libs/armeabi/gdb.setup
    Compile thumb  : hello-jni <= hello-jni.c
    SharedLibrary  : libhello-jni.so
    Install        : libhello-jni.so => libs/armeabi/libhello-jni.so


####可能出现的问题：
如果出现了类似 “Host 'awk' tool is outdated....”这样的错误提示。
只要把prebuilt/linux-x86/bin/下的awk删掉即可
重新编译就OK了</br>
ndk-build


  [1]: https://github.com/sprlee/android-ndk-r8c-linux-x86.git