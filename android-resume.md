# 邵彬 Android 架构师/技术专家

---

# 联系方式

- 手机：18108297138
- 邮箱：shaobin0604@qq.com
- 微信：shaobin0604

---

# 个人信息

- 邵彬/男/1983
- 硕士/本科 天津大学计算机系
- 工作年限：10+ 年
- 技术博客：[http://shaobin0604.cnblogs.com][cnblogs]
- GitHub: [http://github.com/shaobin0604][github]
- Stackoverflow id: shaobin0604
- 期望职位：Android 架构师/技术专家/团队技术负责人
- 期望城市：成都

---

# 工作经历

## 成都运力科技有限公司 2015 年 9 月至今

### 插件框架 Phantom

2016 年 8 月立项，2017 年 1 月投入到生产环境，2018 年 10 开源，详见 [Phantom 项目介绍][Phantom]

### 监控系统

TODO

### 页面统一跳转协议

负责 App 界面之间的串联，即界面跳转服务，支持：

- 宿主原生 Activity
- 插件中的 Activity
- WebViewActivity 打开 URL

优点：

- 将页面映射为 URL ，解偶服务调用者和服务提供者
- 支持外部应用 deeplink 跳转
- 动态配置跳转目标，可做为 hotfix 的一个实现方案

### 客户端升级

TODO

### 表单模板引擎

根据服务端配置的表单，在 Android 端动态生成表单界面。只需要在服务端配置好表单，服务端与客户端均不需要编码，大大减少了业务系统中涉及表单的功能模块（例如：新车、二手车售卖等模块）开发工作量。

- 主导表单模板协议格式设计
- 独立完成 Android 表单模板引擎 SDK ，涉及：
  - 表单模板下载，缓存
  - 渲染引擎
  - 数据绑定

### 研发工程化基础设施建设

#### 代码管理

- 基于 Gerrit/Gitlab + repo ，参考 AOSP 源码管理方式，功能模块代码存放在独立 git 仓库中，方便在各个产品中复用。
- 基础库二进制包发布到内部 maven 仓库

#### 代码 Review

- Gerrit -> Reviewboard -> Gitlab Merge Request

#### 构建系统

基于 Gradle 的构建系统，通过 Product Flavor + Build Type + Build Parameter 实现编译多种版本：

- 测试环境/生产环境
- 集成的各基础库/各插件版本
- 特殊定制版本（包名、主题皮肤、自动化测试包）

#### 持续集成

基于 Jenkins 搭建持续集成方案，涉及

- 执行构建系统编译多种 build virant
- APK 签名
- 应用加固
- 代码质量检查（lint, pmd, findbugs, checkstyle）
- 跟踪包大小，方法数
- 自定义集成的各基础库/各插件版本

#### Release 签名服务

使用远程签名服务替换本地签名机制，杜绝 Keystore 泄漏的风险，提供

1. 测试同学使用的 Web UI
2. 程序集成的 Web Service 接口

#### 多渠道打包服务

基于腾讯 VasDolly 的快速多渠道打包服务，支持 v1/v2 签名，提供

1. 运营使用的 Web UI
2. 程序集成的 Web Service 接口

#### 研发管理

发起并主导以下工作：

- 设计评审
- Code Review
- 技术分享
- 语意化版本命名方案

## 百纳致远（成都）科技有限公司 2013 年 5 月 ~ 2015 年 9 月

### 推送服务 Android 客户端 SDK

- 基于 mqtt 协议的客户端 Paho 实现
- 设计推送消息格式
- 主导推送消息数据统计方案

### 海豚浏览器旋风版

- 下载模块优化。支持多线程分块下载，下载速度提升 30% ~ 50% 。该下载模块同时也在应用商店和视频聚合应用中使用。
- 主题商城模块。支持在线下载主题/皮肤/字体；管理本地安装的主题/皮肤/字体；

### Android 锁屏应用 - One Locker

- 搭建基于 System Window 的应用基础框架
- 技术攻关
  - 屏蔽 状态栏/HOME 键
  - 获取通知消息
  - 获取音乐播放状态，控制音乐播放

### 视频聚合应用 - 快看

- 多线程视频下载模块
- 视频播放模块，破解快播，支持 qvod 协议播放
- 集成第三方广告平台

### 应用商店 - 天翼空间/应用空间/点点市场

- 应用下载模块
- 升级模块
- 卸载反馈模块
- 应用更新检查模块

### 其他项目

- 推进代码质量改进计划，提升团队成员 Code Review 参与度
- 统计团队成员代码贡献的自动化脚本
- Android 客户端团队技术 Wiki 建设，贡献 50+ Wiki

## 北京京联云软件有限公司 2010 年 5 月 ~ 2013 年 5 月

- 带领组员完成基于 AOSP 4.2.2 的 ROM 项目（类似于 MIUI、乐蛙）内置应用程序开发:备份、记事本、手电筒、指南针、文件管理器，录音机、时钟。
- 中移动定制 Android 手机 PC 套件（类似于：豌豆荚、QQ 手机管家）。
- 完整的参与过以下运营商定制手机项目：天语 W606，华为 T8100, 联想 A30T，华为 T8808D，联想 S899t。
- 独立完成中移动 CMMB 手机电视客户端。产品通过中移动运营商测试，目前已有多款上市手机使用该产品，如：华为 T8100, 联想 A30T。
- 3G-324M 视频通话，集成多媒体模块和协议栈模块。
- 多款手机预置应用，如：农历、英汉双解词典、背单词、天气预报。
- Intel Android 2.2 项目，解决 Camera/Multimedia 应用层和框架层的 BUG。

## 云电同方科技有限公司 2008 年 3 月 ~ 2009 年 8 月

- 云南电网电力营销管理信息系统(PMS 3.0)客户端功能模块开发并参与玉溪供电局实施工作。
- 全面业务整合平台(TBI)。该平台整合省电网公司各信息系统的数据资源，提供统一的数据服务接口。
- 昆明供电局营销监控系统。
- 昆明供电局 VIP 客户服务系统。

## IBM 中国软件开发中心 2007 年 7 月 ~ 2008 年 1 月

- 参与 ClearCase 和 ClearQuest 的两个 Patch 版本 7.0.0.2/7.0.1.1 的系统测试工作。

---

# 项目和作品

## 项目

- [Phantom][Phantom] - 零 Hook 稳定占坑类 Android 热更新插件化方案
- [InternetRadio SDK for Android](http://www.cnblogs.com/shaobin0604/archive/2012/12/02/Release-InternetRadio-SDK-for-Android.html) - 用于播放网络流媒体音频的多媒体 SDK 组件
- [HeartbeatFixerForGCM](https://github.com/shaobin0604/HeartbeatFixerForGCM) - 用于解决 GCM 推送延迟问题的小工具
- [Call Vibrator](https://github.com/shaobin0604/CallVibrator) - 类似于 MIUI 系统提供的电话接通/挂断/等待震动功能

## 作品

移步我的 [Google Play 产品列表][googleplay]

# 技能清单

## 熟练使用的技能

- 移动设备开发：Android (SDK/NDK/Framework)
- 数据库相关：SQLite

## 曾经使用的技能

- 移动设备开发：JAVA ME
- Web 开发：Java/Ruby/Python
- Web 框架：Struts/Spring/iBatis/Hibernate/RoR/Sinatra/Flask
- 数据库相关：MySQL
- 搜索：Lucene

---

# 致谢

感谢您花时间阅读我的简历，期待能有机会和您共事。

[cnblogs]: http://shaobin0604.cnblogs.com
[github]: http://www.github.com/shaobin0604
[bitbucket]: http://www.bitbucket.org/shaobin0604
[oschina]: http://git.oschina.net/shaobin0604
[googleplay]: https://play.google.com/store/apps/developer?id=MoboDev
[Phantom]: https://github.com/ManbangGroup/Phantom
