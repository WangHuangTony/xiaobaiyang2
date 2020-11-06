# 6盘小白羊 第二版

开饭中，开源代码已上传  

[11月6日22点20 https://wws.lanzous.com/b01npsg8h](https://wws.lanzous.com/b01npsg8h)  仅供尝鲜,升级时直接替换旧文件即可  

[11月3日15点00 https://wws.lanzous.com/b01nqc4gd](https://wws.lanzous.com/b01nqc4gd)  旧版链接备用  

截止28日，win、linux、mac 均已发布，接下来是完善功能（上传功能），有建议的速提，再接下来要整RSS订阅功能，这是个大项目了。。。。  

[更新日志](ChangeLog.txt)  
#### 2020/11/6
1. Add批量改名功能
2. Add离线任务批量提交多条链接(包括多个BT种子)
3. Add全部任务下载完后自动重试出错任务的机制
4. Add下载完成后调用脚本功能
5. Fix开放远程模式下，复制文件下载链接功能
6. Fix用Safari时BT种子格式化失败的BUG(之前我以为我改好了，其实并没有)
7. 一堆细节上的修正  
  
PS. 最近因为6盘的限制容易下载失败，我已经添加了全部任务下载完后自动重试出错任务的机制。就是全部下载完了没事干了，就自动重新下载之前出错的任务。这样一来，你晚上创建一堆下载，明天一看基本都成功下载了，不像以前会有一些出错没下载完的。  
PS. 左边文件夹树的右键菜单真的好用！！！


### 新版介绍

采用vue+antd开发UI界面，go开发后台服务程序。无需安装，启动后调用浏览器显示UI和操作。支持win/linux/mac全平台，支持远程管理  

### 版权声明

6盘小白羊版仅是完全免费的个人学习作品，和6盘官方无任何关联。所有功能均基于调用6盘官方开放API，再此感谢6盘的无私。6盘官网地址为  **6pan.cn** 

### 新版功能

6盘官方网页版功能已基本覆盖

``` diff
+ [√] 登录6盘账号(支持 手机+密码、用户名+密码、粘贴Cookie 三种方式)
+ [√] 文件功能：文件列表+排序、移动、复制、重命名、获取下载地址、删除到回收站
+ [√] 回收站功能：文件列表、恢复文件、彻底删除文件、清空回收站
+ [√] 离线下载功能：任务列表、查看复制离线任务链接、删除离线任务、添加离线任务
+ [√] 用户功能：个人信息、修改密码、WEBDAV信息
+ [√] 6盘官方公告
+ [√] 文件搜索
- [x] 手机绑定、其他网盘推送、删除账户、工单系统、订阅系统、分享系统 都会被屏蔽，不计划实现这些功能
```

小白羊第二版特色功能

``` diff
+ [√] 多账号同时登录管理
+ [√] 目录树快捷导航(包括右键菜单快捷操作)
+ [√] 文件、文件夹批量下载
+ [√] 图片预览(单图片预览、文件夹全部图片预览)
+ [√] 音视频在线播放(调用本地VLC播放器，支持.mp4.mkv所有常见格式，支持win/linux/mac os，支持用其他播放器替代)
+ [√] 文本小文件在线预览(.txt .css .js等)
+ [√] 文件批量重命名
+ [√] 界面美化(文件图标、操作步骤简化)
+ [√] 自研下载引擎：多文件同时下载，每个文件都会多线程并发下载，提升下载速度。
+ [√] 文件下载支持断点续传，不受6盘下载链接时效限制，可以下载大文件（20-30GB单文件）
+ [√] 文件下载完可以自动执行脚本文件回调（完全参照aria2）
# [*] 文件上传功能：支持多文件、文件夹批量上传，支持断点续传，支持文件秒传功能
+ [√] 多平台支持：支持windows，linux(ubuntu，centos等等)，mac os
+ [√] 远程管理功能：支持通过在浏览器输入IP，远程管理
- [ ] RSS订阅功能：~~订阅资源秒传~~
```
*注：+ [√] 是已经开发完毕可以使用的功能  
*注：小白羊第二版已去除内置账号，请用户使用自己的6盘VIP账号提交百度分享任务  
*注：小白羊第一版因为6盘官方限制并发数太严格，如果你的网速很快，会遇到下载一段时间后速度为0，等1-2分钟后才能恢复下载的BUG。第二版已修此问题  

### 特别备注

1. 6盘是一个网盘，免费用户每天可以离线3个任务（BT、磁力、电驴、HTTP、FTP）；付费用户每天可以离线100个任务（+支持百度分享链接）
2. 小白羊版只是UI，你离线是保存到6盘中，下载文件是从6盘下载，付费订阅是指付费订阅6盘官网的会员服务。小白羊只是6盘美化版UI，请正确认知
3. 小白羊版会长期维护

截图：（看不到是网络原因,大陆github就是卡）  
  
![demo1015](demo1015.png)
