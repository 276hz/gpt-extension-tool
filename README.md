<div align="center">

# ChatGPT Session Helper Extension

### Browser Session Research & JSON Export Toolkit  
### 浏览器 Session 研究与 JSON 导出工具

<img src="./icon.png" width="120" />

<br/>

![Manifest V3](https://img.shields.io/badge/Manifest-V3-10a37f)
![Chrome Extension](https://img.shields.io/badge/Chrome-Extension-blue)
![JavaScript](https://img.shields.io/badge/JavaScript-ES2023-yellow)
![Status](https://img.shields.io/badge/Status-Experimental-orange)
![License](https://img.shields.io/badge/License-MIT-black)

</div>

---

# Overview / 项目简介

A lightweight Chrome Extension for learning and testing browser session workflows on ChatGPT pages.

一个轻量级 Chrome 扩展，用于学习和测试 ChatGPT 页面中的浏览器 Session 工作流程。

This project demonstrates:

本项目演示：

- Chrome Extension Manifest V3 architecture  
  Chrome Extension Manifest V3 架构

- Browser scripting APIs  
  浏览器脚本 API

- Frontend session handling  
  前端 Session 处理

- Clipboard interaction  
  剪贴板交互

- JSON export workflows  
  JSON 导出流程

---

# Preview / 预览

```text
ChatGPT Web
     ↓
Browser Extension
     ↓
Session Extraction
     ↓
Structured JSON
     ↓
Clipboard Export
```

---

# Features / 功能特性

## Core Features / 核心功能

- Detect active ChatGPT tab  
  检测当前 ChatGPT 页面

- Inject scripts into webpage context  
  向网页上下文注入脚本

- Export structured JSON data  
  导出结构化 JSON 数据

- Clipboard auto-copy support  
  自动复制到剪贴板

- Lightweight popup UI  
  轻量级弹窗界面

- Manifest V3 compatible  
  支持 Manifest V3

---

# Tech Stack / 技术栈

| Technology | Description |
|---|---|
| JavaScript | Main logic |
| HTML/CSS | Popup UI |
| Chrome Extension API | Browser integration |
| Manifest V3 | Extension architecture |

---

# Project Structure / 项目结构

```text
.
├── manifest.json
├── popup.html
├── popup.js
├── icon.png
└── README.md
```

| File | Description | 说明 |
|---|---|---|
| manifest.json | Extension configuration | 扩展配置 |
| popup.html | Popup interface | 弹窗页面 |
| popup.js | Main logic | 主逻辑代码 |
| icon.png | Extension icon | 扩展图标 |

---

# Installation / 安装方法

## Chrome / Edge

### 1. Clone Repository / 克隆仓库

```bash
git clone https://github.com/276hz/gpt-extension-tool.git
```

Or download ZIP manually.  
或者手动下载 ZIP 文件。

---

### 2. Open Extensions Page / 打开扩展页面

Chrome:

```text
chrome://extensions/
```

Edge:

```text
edge://extensions/
```

---

### 3. Enable Developer Mode / 开启开发者模式

Enable:

```text
Developer Mode
```

(top-right corner)

右上角开启开发者模式。

---

### 4. Load Extension / 加载扩展

Click:

```text
Load unpacked
```

Select the project folder.

选择项目目录即可。

---

# Usage / 使用方法

## Basic Workflow / 基础流程

1. Open ChatGPT webpage  
   打开 ChatGPT 页面

2. Click extension icon  
   点击扩展图标

3. Press extract button  
   点击提取按钮

4. JSON data will be copied to clipboard  
   JSON 数据会自动复制到剪贴板

---

# Architecture / 架构说明

## Browser Workflow / 浏览器工作流程

```text
popup.html
    ↓
popup.js
    ↓
chrome.scripting.executeScript
    ↓
Injected Page Context
    ↓
Frontend Session Data
    ↓
JSON Export
```

---

# Permissions / 权限说明

| Permission | Purpose | 用途 |
|---|---|---|
| activeTab | Access active tab | 访问当前标签页 |
| scripting | Inject scripts | 注入脚本 |
| host_permissions | Access ChatGPT pages | 访问 ChatGPT 页面 |

---

# Browser Compatibility / 浏览器兼容性

| Browser | Support |
|---|---|
| Chrome | ✅ |
| Edge | ✅ |
| Brave | ✅ |
| Opera | ⚠️ Partial |
| Firefox | ⚠️ Requires Modification |
| Safari | ❌ |

---

# Development / 开发说明

## Reload Extension / 重载扩展

After editing source code:

修改源码后：

1. Open extensions page  
2. Click reload button  
3. Refresh ChatGPT webpage  

---

# Security Notes / 安全说明

## Important / 重要提示

This repository is intended for:

本仓库仅用于：

- browser extension learning  
  浏览器扩展学习

- frontend research  
  前端研究

- development experiments  
  开发实验

Please DO NOT:

请不要：

- publish sensitive session data  
  公开敏感 Session 数据

- upload personal credentials  
  上传个人凭证

- expose browser tokens publicly  
  公开浏览器 Token

---

# Manifest Version / Manifest 版本

This project uses:

本项目使用：

```json
{
  "manifest_version": 3
}
```

Manifest V3 introduces:

Manifest V3 特性：

- modern scripting APIs  
  现代脚本 API

- stricter permission handling  
  更严格的权限管理

- improved extension security  
  更高的扩展安全性

---

# Clipboard API / 剪贴板 API

Example:

```js
navigator.clipboard.writeText(...)
```

Some browsers may restrict clipboard access.  
部分浏览器可能限制剪贴板权限。

---

# Troubleshooting / 常见问题

## Extension Not Working / 扩展无法运行

Try:

- refreshing ChatGPT page  
- reloading extension  
- checking browser permissions  

尝试：

- 刷新 ChatGPT 页面
- 重载扩展
- 检查浏览器权限

---

## Clipboard Copy Failed / 自动复制失败

Some browsers block clipboard APIs.

部分浏览器可能阻止剪贴板 API。

Fallback textarea copy is included.

项目已包含备用复制方案。

---

# Future Improvements / 后续计划

- Better popup UI  
- Dark mode  
- Multi-language support  
- Better error handling  
- Configurable export formats  
- Firefox compatibility  

---

# Disclaimer / 免责声明

This repository is provided for educational and development purposes only.

本仓库仅用于学习与开发测试。

This project is NOT affiliated with OpenAI.

本项目与 [OpenAI](https://openai.com?utm_source=chatgpt.com) 无官方关联。

Users are responsible for complying with all applicable terms and policies.

用户需自行遵守相关平台条款与政策。

---

# License / 开源协议

MIT License © 2026
