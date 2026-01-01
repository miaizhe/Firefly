---
title: WuXi-Player 正式发布
published: 2026-01-01
description: '一个现代、简约且功能强大的音乐播放器 —— WuXi-Player 正式发布！'
image: './images/firefly.webp'
tags: [开源项目, 音乐播放器, WuXi-Player, JavaScript]
category: '项目动态'
draft: false
---

## 🎵 项目简介

**WuXi-Player** 是一款致力于提供极致听歌体验的现代音乐播放器。它结合了简约的设计语言与强大的功能，旨在为用户打造一个纯净、高效的音频播放环境。

目前项目已在 GitHub 正式开源！

### ✨ 核心特性

- **现代 UI 设计**：采用简约而不简单的视觉风格，适配多种屏幕尺寸。
- **高性能播放引擎**：基于 APlayer 构建，支持多种音频格式。
- **Meting API 集成**：无缝对接网易云音乐、QQ音乐等主流平台歌单。
- **高度可定制**：支持主题色调节、看板娘交互等个性化设置。
- **轻量化**：极小的资源占用，极速的加载体验。

---

## 🔗 相关链接

- **GitHub 仓库**: [miaizhe/WuXi-Player](https://github.com/miaizhe/WuXi-Player)
- **在线演示**: [点击查看](https://eo.wu-xi.xyz/)

::github{repo="miaizhe/WuXi-Player"}

---

## 🚀 快速开始

如果你想在自己的项目中使用 WuXi-Player，可以参考以下代码：

```html
<script src="https://cdn.jsdelivr.net/gh/miaizhe/WuXi-Player/dist/WuXi-Player.min.js"></script>
<div id="wuxi-player"></div>
<script>
  const player = new WuXiPlayer({
    container: document.getElementById('wuxi-player'),
    audio: {
      name: '歌曲名',
      artist: '艺术家',
      url: '音频链接',
      cover: '封面链接'
    }
  });
</script>
```

欢迎大家前往 GitHub 提交 Issue 或 Pull Request，一起完善这个项目！
