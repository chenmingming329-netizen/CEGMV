# TikTok GMV Max 广告管家 v1.5：素材 Dashboard + 素材评分分级

本版把 v1.3 的素材定时监控升级成：

1. 素材 Dashboard 面板：`http://127.0.0.1:8774/creative-dashboard`
2. 素材 S/A/B/C/D/E 自动评分分级
3. 自动生成 `creative_score.csv`
4. 自动生成 `creative_advice.txt`
5. 保留素材定时监控：无变化不重复发送，只在重要变化时发送
6. 保留“刷新当前素材页并填入 / 发送”按钮
7. 保留 GMV Max 计划体检和 GMV 面板

## 安装

1. 解压本文件夹
2. Chrome 打开 `chrome://extensions/`
3. 移除旧版插件
4. 加载本文件夹：`browser_agent_extension_v15_creative_dashboard_score`
5. 双击 `kill_8774_then_start.bat`

正常看到：

```text
本地管家已启动：http://127.0.0.1:8774
素材Dashboard：http://127.0.0.1:8774/creative-dashboard
```

## 素材使用方式

1. 打开 TikTok：广告计划数据分析 > 创意素材
2. 点插件：`保存当前素材页地址`
3. 等待秒数建议先设置：`30`
4. 点：`刷新当前素材页并填入`
5. 确认字段正常后，再点：`刷新当前素材页并发送`
6. 查看素材面板：`打开素材Dashboard`

## 生成文件

每次素材采集会生成：

```text
creative_items.csv
creative_diagnosis.csv
creative_score.csv
creative_score.json
creative_advice.txt
creative_change.json
chatgpt_message.txt
screenshot.png
page_text.txt
```

## 素材等级说明

```text
S：重点保留 + 复制重拍
A：保留观察 + 复制备份
B：继续观察 / 优化落地页
C：小样本继续观察
D：暂停 / 换素材
E：商品卡片或字段异常，不参与诊断
```

## 推荐下一步

先用“只保存到本地，不发 ChatGPT”跑 1-2 轮，确认 Dashboard 分级合理后，再开启“有变化时填入 ChatGPT，等我确认发送”。
