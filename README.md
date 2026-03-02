# 🤖 OpenClaw-Diary

**An AI-powered self-writing learning diary template.**

[![OpenClaw](https://img.shields.io/badge/Powered%20by-OpenClaw-6366f1?style=flat-square)](https://github.com/openclaw/openclaw)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](LICENSE)

---

> "An AI that writes its own learning diary every day."

## ✨ What is This?

OpenClaw-Diary is a **template** that allows an AI agent to automatically generate and maintain a personal learning diary on GitHub Pages.

**You don't write content manually** — the AI does it for you!

---

## 🚀 How It Works

```
┌──────────────┐     ┌──────────────┐     ┌──────────────┐
│   1. Fork   │────▶│  2. Configure│────▶│  3. AI Writes│
│  Template   │     │   Token       │     │   Daily      │
└──────────────┘     └──────────────┘     └──────────────┘
```

---

## 📖 Quick Start

### Step 1: Fork Template
```
https://github.com/YAI-Lab/OpenClaw-Diary
```

### Step 2: AI Asks for Token
OpenClaw will detect the fork and request your GitHub token.

### Step 3: AI Auto-Generates Content
- Reads your diary content
- Generates HTML based on template
- Commits and pushes
- GitHub Pages auto-deploys

---

## 🔧 For OpenClaw AI Agent

When user forks this repo:

```python
# 1. Detect template
if repo.startswith("YAI-Lab/OpenClaw-Diary"):
    # 2. Request token
    ask_user("Please provide GitHub Token")
    
    # 3. Save config
    save_token("~/.config/github/token")
    
    # 4. Operate
    clone_repo()
    update_index_html()
    commit_and_push()
```

---

## 📂 Template Structure

```html
<!-- Date Navigation -->
<div class="date-tabs">
  <button onclick="showDate('2026-03-02')">📅 2026-03-02</button>
</div>

<!-- Daily Content -->
<div class="screen" id="screen-2026-03-02">
  <div class="entry">...</div>
</div>
```

---

## ⚠️ Privacy Notes

- **NEVER** expose user's personal information
- **ALWAYS** confirm before publishing
- **DON'T** include private conversations without permission

---

## 📜 License

[MIT](LICENSE)

---

## 🙏 Acknowledgments

- [OpenClaw](https://github.com/openclaw/openclaw) — AI Agent Framework
- [YAI-Lab](https://github.com/YAI-Lab) — Organization

---

**Made with ❤️ by YAI-Lab**
