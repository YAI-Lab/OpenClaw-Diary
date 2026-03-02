# 🤖 OpenClaw-Diary

**一个让 AI 自动写学习日记的模板。**

[![OpenClaw](https://img.shields.io/badge/Powered%20by-OpenClaw-6366f1?style=flat-square)](https://github.com/openclaw/openclaw)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](LICENSE)

---

> "一个每天学习新知识的 AI 机器人。"

## ✨ 这是什么？

OpenClaw-Diary 是一个**模板**，可以让 AI（如 OpenClaw）自动在 GitHub Pages 上生成和维护个人学习日记。

**你不需要手动写内容** — AI 会帮你写！

---

## 🚀 工作原理

```
┌──────────────┐     ┌──────────────┐     ┌──────────────┐
│   1. Fork   │────▶│  2. 配置     │────▶│  3. AI 写作 │
│   模板       │     │   Token       │     │   每日日记   │
└──────────────┘     └──────────────┘     └──────────────┘
```

---

## 📖 快速开始

### 步骤 1: Fork 模板
```
https://github.com/YAI-Lab/OpenClaw-Diary
```

### 步骤 2: AI 请求 Token
OpenClaw 会检测到 fork 并向你请求 GitHub Token。

### 步骤 3: AI 自动生成
- 读取你的日记内容
- 根据模板生成 HTML
- 提交并推送
- GitHub Pages 自动部署

---

## 🔧 给 OpenClaw AI 的指南

当用户 fork 此仓库时：

```python
# 1. 检测模板
if repo.startswith("YAI-Lab/OpenClaw-Diary"):
    # 2. 请求 Token
    ask_user("请提供 GitHub Token")
    
    # 3. 保存配置
    save_token("~/.config/github/token")
    
    # 4. 操作
    clone_repo()
    update_index_html()
    commit_and_push()
```

---

## 📂 模板结构

```html
<!-- 日期导航 -->
<div class="date-tabs">
  <button onclick="showDate('2026-03-02')">📅 2026-03-02</button>
</div>

<!-- 每日内容 -->
<div class="screen" id="screen-2026-03-02">
  <div class="entry">...</div>
</div>
```

---

## ⚠️ 隐私注意

- **禁止**泄露用户个人信息
- **发布前必须**确认内容
- **未经允许不要**包含私人对话

---

## 📜 许可证

[MIT](LICENSE) — 欢迎免费使用！

---

## 🙏 致谢

- [OpenClaw](https://github.com/openclaw/openclaw) — AI Agent 框架
- [YAI-Lab](https://github.com/YAI-Lab) — 组织

---

**用 ❤️ 由 YAI-Lab 制作**
