---
title: "RN运行报错日志记录集"
date: 2020-04-26T11:04:20+08:00
draft: true
---

整理了这两年开发rn过程中，记录了的一些，遇到的运行相关的问题。

1. [友盟iOS13报错([_LSDefaults sharedInstance] unrecognized selector sent to class)](http://note.youdao.com/noteshare?id=56f25e41d1ae0fef7581a03c22b5cd92)


2. [Could not launch “XXX” Domain IDEDebugSessionErrorDomain](http://note.youdao.com/noteshare?id=a6d500b937230779049524bce2e7c7db)


3. [Cannot fit requested classes in a single dex file](http://note.youdao.com/noteshare?id=e916ffe40a7d16396b165d2e4e8594bb)


4. [react-native android报错找不到相应模块解决办法](http://note.youdao.com/noteshare?id=e6349dd07bbd289330901d1f15df14ee)


5. [ios连接真机调试的时候打不开debug模式](http://note.youdao.com/noteshare?id=7cd87f43a91251515030424e4035ce38)


6. [RN0.57打包报错，Execution failed for task ‘xxx，verifyReleaseResources'](http://note.youdao.com/noteshare?id=2afccb797f0ba6ebad16c0faf7247d47)


7. [执行react-native run-android报错](http://note.youdao.com/noteshare?id=b199fecaa64b9ae5a7862abdaa6b6e0d)


8. [FileProvider冲突报错(现有的代码拉下来就会有这个问题，因为加了下载更新相关的代码导致)](http://note.youdao.com/noteshare?id=d242c87f075b8762ccec330c864cbce8)


9. [react native android studio 报错R文件丢失](http://note.youdao.com/noteshare?id=be218e6ad56f78e601ee9359d32800bd)


10. [IOS打包报重复引用问题](http://note.youdao.com/noteshare?id=ca07faaf259887bc7eb2ae1bee6efc63)


11. [react native android4.4开启debug模式无效问题](http://note.youdao.com/noteshare?id=1689f0ac9b781cf468b9700cc0df5c6a)


12. [react-native run-android运行完，开启debug模式metro bundle报错](http://note.youdao.com/noteshare?id=3e2bbcfda4dfddab9dbc511603e74e98)


13. [react-native run-android报错](http://note.youdao.com/noteshare?id=7a10ba38769f1c7546249b7a4c699a25)


14. [React Native 日常报错 'config.h' file not found](http://note.youdao.com/noteshare?id=f9c44683ee4ba75c8f003f3a81c580ac)


15. [android 编译报错 Could not find support-compat.aar (com.android.support:support-compat:27.1.0)](http://note.youdao.com/noteshare?id=b96388a5ccc0b33f6107d4499c2fd0ae)


16. [android报错：Only fullscreen activities can request orientation](http://note.youdao.com/noteshare?id=5654116592cfacf14fd4d52e3002b6e1)


17. [React Native报错：Error recordAsync Expected a Camera component](http://note.youdao.com/noteshare?id=3c8d223d1ad0dc808c53e07517d13855)


18. [react-native run-android运行报错说找不到设备（权限问题）](http://note.youdao.com/noteshare?id=830c4c077ee361a0575ad2361cc6de8b)


19. [打包常见错误](http://note.youdao.com/noteshare?id=7392c313d2ab61c9d71bf227946b881e)


20. [安装启动遇到的问题](http://note.youdao.com/noteshare?id=f0ccc6a63e9fb22e1ba0bdde8ed18da9)


21. android 真机运行，报错找不到bundle.js文件，解决办法：(这个不是最好的解决办法，具体的我还有点记不太清了)
Unable to load script from assets 'index.android.bundle' ？
解决办法：
在android\app\src\main\下新建assets文件夹，然后执行：
react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res
会在assets下面生成index.android.bundle和index.android.bundle.meta文件
最后重新运行：react-native run-android
就可以了。

22. [android真机运行可以了，开启remote debug调试报错](https://reactnative.cn/docs/0.51/running-on-device-android.html)
运行:
`adb reverse tcp:8081 tcp:8081`