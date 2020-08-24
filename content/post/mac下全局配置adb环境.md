---
title: "mac下全局配置adb环境"
date: 2020-07-01
draft: true
---
# 前言
adb的全称为Android Debug Bridge，就是起到调试桥的作用。通过adb我们可以在IDE中通过DDMS来调试Android程序，其实也就是debug工具。

但是我们在MAC下安装完JDK和Android studio以后，我们在命令行执行这个命令，会提示这个错误：
`adb: command not found`

# Android adb环境设置

- 进入当前用户home目录
打开terminal终端，默认就是home根目录。如果不确认，可以在命令行输入：
`echo $HOME`

输出的内容一般是类似这样的信息：/Users/你自己的用户名
也可以使用以下命令，查看当前所在目录：
`pwd`

- 创建.bash_profile文件
`touch .bash_profile`

- 打开.bash_profile文件
`open -e .bash_profile`

- 编辑.bash_profile文件。注意：/Users/你自己的用户名 要换成你自己的home目录
```
export ANDROID_HOME=/Users/你自己的用户名/Library/Android/sdk
export PATH=${PATH}:${ANDROID_HOME}/tools
export PATH=${PATH}:${ANDROID_HOME}/platform-tools
```

- 编译.bash_profile
`source .bash_profile`

- 至此adb环境已经搭建成功，可以输入以下命令做个验证：
`adb version`
会输出类似以下信息：
```
Android Debug Bridge version 1.0.41
Version 29.0.6-6198805
Installed as /Users/你自己的用户名/Library/Android/sdk/platform-tools/adb
```