# DesignTube

**看懂设计背后的为什么。**

DesignTube 是一个给设计师的 YouTube：不教软件、不追热点，只收录那些讨论设计如何影响人、审美为何流行、经典为何经典的视频。没有算法推荐，没有点击诱饵，不需要账号。

灵感来自 Andrej Karpathy 的 [HackerTube](https://hackertube.org)。它收录的是 Hacker News 上被反复推荐的 YouTube 视频，DesignTube 把同样的思路用在设计上。

## 五个问题

片单围绕五个问题组织：

1. 设计如何影响人的行为？
2. 为什么某种审美会在特定时代流行？
3. 技术变革如何改变视觉语言？
4. 一个品牌如何建立自己的辨识度？
5. 为什么有些设计能够跨越时代？

另有三个专题：**设计师演讲**（TED 与各大设计会议）、**乔布斯**、**AI 与审美**。

目前收录 49 部视频，讲者包括 Don Norman、Paula Scher、Tony Fadell、Stefan Sagmeister、Michael Bierut、John Maeda、Dieter Rams、Massimo Vignelli、Saul Bass、Charles & Ray Eames、Susan Kare、原研哉、Jony Ive、Steve Jobs 等。

## 功能

- **筛选**：按年代、类型、主题、特色筛选，可按精选顺序、年份或随机排序
- **真实视频帧作封面**：用视频中间的一帧当封面，而不是标题党缩略图（加载失败时显示按主题生成的排版封面）
- **站内播放，自带中文字幕**：使用 YouTube 自带字幕；没有中文字幕的视频会自动翻译成中文，可切换简体、繁體、原文或关闭
- **每部视频都有推荐理由和思考题**：“看之前想一想”
- **无账号**：赞、踩、稍后观看、历史记录都只保存在你自己的浏览器里
- **深色模式**、键盘快捷键（`/` 搜索，`R` 随机一部）
- **导出数据**：一键复制全部片单 JSON，交给 AI agent 做你自己的版本

## 技术

整个站点就是一个静态文件 `index.html`，不需要构建，也没有依赖。视频托管在 YouTube，本站只做整理和展示。

```
index.html    站点本身（数据、样式、脚本都在里面）
vercel.json   Vercel 部署配置
```

## 路线图

- [ ] 像 HackerTube 一样，从设计社区（Hacker News、Reddit 设计版块、Designer News 等）挖掘被反复推荐的视频，代替人工片单
- [ ] 用 YouTube Data API 补全时长、播放量
- [ ] 按时长筛选、“隐藏好片”（推荐多但播放少）

## 声明

本项目与 YouTube、Google 及 HackerTube 无关。所有视频版权归原作者所有，本站仅提供链接与嵌入播放。
