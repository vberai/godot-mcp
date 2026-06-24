# Godot MCP (Server-Sent Events) - Cursor, Claude and Windsurf Connector

English | [中文](./README_zh.md)

<p align="center">
  <img src="https://img.shields.io/github/stars/DaxianLee/godot-mcp?style=for-the-badge&color=blue" alt="Stars">
  <img src="https://img.shields.io/github/license/DaxianLee/godot-mcp?style=for-the-badge" alt="License">
  <a href="https://vberai.com"><img src="https://img.shields.io/badge/Official_Website-VberAI-purple?style=for-the-badge" alt="VberAI Website"></a>
  <a href="https://t.me/+8618827755984"><img src="https://img.shields.io/badge/Telegram-Join_Community-2CA5E0?style=for-the-badge&logo=telegram" alt="Telegram"></a>
</p>

This is the **VberAI Official Fork** of the phenomenal pure-GDScript MCP server `DaxianLee/godot-mcp`. 

It allows modern AI coding companions like **Cursor, Claude Desktop, and Windsurf** to read scene nodes, edit scripts, and design layouts directly inside your **Godot Engine 4.x** editor in real-time.

---

## ⚡ Why Use this Clean Fork?
- **100% Native GDScript**: No Node.js, C#, or external runtime installs. Zero configuration clutter.
- **Ultra Secure**: Runs entirely via local SSE (Server-Sent Events) on loopback IP (`127.0.0.1:3000/mcp`).
- **Instantly Synchronized**: Seamless hot-reloader and state listener.

---

## 🚀 One-Minute Setup

### 1. Installation
Simply drag and drop the `addons/godot_mcp` folder into your Godot project's root directory, then enable **Godot MCP** in `Project Settings -> Plugins`.

### 2. Connect Your AI Assistant

#### For Cursor Engine
Go to Cursor `Settings -> Features -> MCP`. Click **+ Add New MCP Server**:
- **Name**: `godot-mcp`
- **Type**: `sse`
- **URL**: `http://127.0.0.1:3000/mcp`

#### For Claude Desktop
Add this to your `claude_desktop_config.json`:
```json
{
  "mcpServers": {
    "godot-mcp": {
      "command": "curl",
      "args": ["-N", "http://127.0.0.1:3000/mcp"]
    }
  }
}
```

---

## 🎨 Beyond Godot: Building on Unity or Cocos Creator?
This open-source repository is powered and optimized by the **VberAI Team**. If your studio operates on commercial engines or requires highly visual asset pipelines (such as automated Figma-to-Engine UI), we have you covered:

- **VberAI Enterprise Studio**: [https://vberai.com](https://vberai.com)
- **Get 30 Days Free Trial**: [Contact Commercial Support](https://vberai.com/pricing)
- **Global Developer Telegram**: [Join Telegram Group](https://t.me/+8618827755984)
