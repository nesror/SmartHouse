# SmartHouse

A Home Assistant third-party client built with Flutter. Faster startup and friendlier operation.  
基于 Flutter 的 Home Assistant 第三方客户端，启动更快、操作更友好。  
How to use（使用教程）：[bilibili](https://www.bilibili.com/video/BV16WCbYwEaH/)

- Home and Introduction （主页与介绍）
  - https://191005.xyz/smarthouse/
- Download 下载：
  - [App Store](https://apps.apple.com/app/id6753762531)
  - [Google Play](https://play.google.com/store/apps/details?id=cn.yzapp.flutter.ha)
- Change log 更新日志
  - [bilibili 介绍](https://www.bilibili.com/video/BV1Y8411179b/)
  - [订阅号更新日志](https://mp.weixin.qq.com/s/Fce0EhnMYU-uy96yIH9_0A)
- Mini version 精简版（无本地 HA GUI）
  - [Release (app-mini-release.apk)](https://github.com/nesror/SmartHouse/releases/latest)

---

# SmartHouse (Home Assistant Flutter Client)

这是一个基于 Flutter 的 Home Assistant 客户端。

## 项目定位

- 面向 Home Assistant 用户的移动端客户端。
- 提供设备控制、语音助手、媒体浏览、历史查看、传感器上报、通知联动等能力。
- 支持多服务地址切换（外网/内网）、WebView 登录、原生通知监听和前台服务。

## 核心功能

- **Home Assistant 登录与连接**
  - 支持 `Long-Lived Access Token` 登录。
  - 支持 WebView 密码登录并自动提取 `hassTokens`。
  - 支持多服务地址管理与切换（`ServiceChooseScreen`）。
- **首页设备控制**
  - 自动拉取实体并按 Tab 组织展示。
  - 支持灯光、风扇、空调、窗帘、媒体、摄像头等常见域。
  - 支持实体卡片编辑、排序、固定消息实体。
- **Assist 对话与语音**
  - 基于 HA `assist_pipeline` 的文本对话。
  - 语音输入支持系统 STT/TTS 与 Sherpa ONNX（离线模型）。
  - 可选择当前 Assist Pipeline。
- **媒体与历史**
  - 支持 HA 媒体源浏览、应用内播放/查看、外部打开。
  - 支持实体历史记录查看。
- **配置与个性化**
  - 主题色与深色模式。
  - Dashboard 配置同步与本地保存。
  - 通知实体、消息实体、Tab 配置。
- **传感器与通知联动（Android 重点）**&#8203;
  - 前台服务定时上报电量、Wi-Fi、步数、BLE、定位。
  - 原生通知监听服务回传通知内容到 HA。
  - 推送动作可触发实体跳转、媒体打开、服务调用。
- **设备本地 Home Assistant 安装（Android）**&#8203;
  - 无需电脑与服务器，直接在本机下载并运行 Home Assistant 容器（基于 proot，无 root）。
  - 内置大陆可访问的镜像源与自动回退，安装进度实时反馈、失败可重试、完成后自动启动服务。
