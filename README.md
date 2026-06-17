# TikTok GMV Max Ad Manager

本项目是一个本地浏览器插件 + Python 本地管家，用于辅助监控 TikTok GMV Max 广告计划和创意素材数据。

## 当前版本

`v1.5 Creative Dashboard + Score`

## 核心功能

- GMV Max 计划数据采集
- 创意素材页面采集
- 素材定时监控
- 素材变化对比
- 素材 S/A/B/C/D/E 自动评分分级
- 本地素材 Dashboard 面板
- 可选择只保存到本地、填入 ChatGPT、或发送到 ChatGPT 复核

## 本地面板

```text
http://127.0.0.1:8774/creative-dashboard
```

## 安全说明

本仓库只上传工具源码和说明，不包含：

- TikTok Cookie
- TikTok Token
- 账号密码
- API Key
- 真实广告数据快照
- 本地 snapshots 采集结果

## 安装方式

1. 下载或克隆本仓库
2. 打开 Chrome：`chrome://extensions/`
3. 开启「开发者模式」
4. 点击「加载已解压的扩展程序」
5. 选择本仓库文件夹
6. 双击运行：`kill_8774_then_start.bat`
7. 打开 TikTok GMV Max 创意素材页面后使用插件

## 备注

这是内部运营辅助工具，页面结构变化时可能需要继续维护解析逻辑。
