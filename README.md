# 🤖 Claude Code

<p align="center">
  <img src="https://img.shields.io/badge/TypeScript-5.1+-3178C6?style=flat&logo=typescript" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Bun-1.3.5+-FBE078?style=flat&logo=bun" alt="Bun" />
  <img src="https://img.shields.io/badge/Node.js-24+-339933?style=flat&logo=node.js" alt="Node.js" />
  <img src="https://img.shields.io/badge/License-Anthropic-FF6B6B?style=flat" alt="License" />
</p>

<br/>

<p align="center">
  <a href="#快速开始">🚀 快速开始</a> •
  <a href="#功能特性">✨ 功能特性</a> •
  <a href="#技术栈">🛠 技术栈</a> •
  <a href="#项目结构">📁 项目结构</a> •
  <a href="#贡献指南">🤝 贡献</a>
</p>

<br/>

---

## 📖 简介

| |
|:---|
| **Claude Code** 是 Anthropic 推出的 AI 编程助手 CLI 工具，提供强大的代码编辑、任务自动化和智能辅助功能。 |
| 本项目是 Claude Code 源码的恢复版本，通过 source map 逆向还原并补齐缺失模块后得到的完整源码树。 |

---

## ⚡ 快速开始

```bash
# ══════════════════════════════════════════════
#  📦 安装依赖
# ══════════════════════════════════════════════
bun install

# ══════════════════════════════════════════════
#  🚀 运行 CLI
# ══════════════════════════════════════════════
bun run dev

# ══════════════════════════════════════════════
#  🔖 查看版本
# ══════════════════════════════════════════════
bun run version
```

---

## ✨ 功能特性

<div align="center">

| 🧠 | ⚡ | 🔌 | 💾 | 🔒 | 🐛 |
|:---:|:---:|:---:|:---:|:---:|:---:|
| **智能代码编辑** | **任务自动化** | **MCP 集成** | **会话管理** | **权限系统** | **调试能力** |
| AI 驱动的代码补全、重构和建议 | 支持复杂的多步骤任务规划和执行 | 完整的 Model Context Protocol 支持 | 强大的会话历史和状态管理 | 精细化的工具调用权限控制 | 内置调试工具和日志系统 |

</div>

---

## 🛠 技术栈

```
┌──────────────────────────────────────────────────────────────┐
│                     🖥️  Tech Stack                            │
├──────────────────────────────────────────────────────────────┤
│                                                              │
│   ┌──────────────┐                                           │
│   │   🟣 Bun     │  Package Manager                          │
│   └──────┬───────┘                                           │
│          │                                                    │
│          ▼                                                    │
│   ┌──────────────┐                                           │
│   │ 🟢 Node.js   │  Runtime Engine (≥24.0.0)                │
│   │    24+       │                                           │
│   └──────┬───────┘                                           │
│          │                                                    │
│    ┌─────┴─────┬──────────┬───────────┬──────────┐          │
│    ▼           ▼          ▼           ▼          ▼          │
│   SDK       SDK        Protocol    Telemetry    UI         │
│  Anthropic  Claude     MCP        OpenTelemetry  React     │
│              Agent                                  +Ink    │
│                                                              │
└──────────────────────────────────────────────────────────────┘
```

---

## 📁 项目结构

```
.
│
├── 📂 src/                     ⭐ 核心源代码
│   ├── bridge/                🚪 桥接层 (外部通信)
│   ├── assistant/             🧠 助手核心逻辑
│   ├── bootstrap/             🚀 启动引导
│   ├── skills/                ⚡ 技能系统
│   └── ...
│
├── 📂 shims/                  🔧 兼容层 (Native Bindings)
│
├── 📂 vendor/                 📚 第三方源码
│
├── 📄 AGENTS.md               📝 Agent 配置规范
│
└── 📦 package.json            ⚙️  项目配置
```

---

## 🧩 可用命令

<div align="center">

| 命令 | 说明 | 状态 |
|:---|:---|:---:|
| `bun run dev` | 开发模式运行 | ✅ |
| `bun start` | 生产模式运行 | ✅ |
| `bun run version` | 查看版本信息 | ✅ |
| `bun run dev --help` | 查看帮助文档 | ✅ |

</div>

---

## 📌 环境要求

<div align="center">

```
┌─────────────────────────────────────┐
│           🖥️  Requirements          │
├─────────────────────────────────────┤
│                                     │
│   🟣  Bun        │   ≥ 1.3.5       │
│   ──────────────┼─────────────     │
│   🟢  Node.js   │   ≥ 24.0.0      │
│                                     │
└─────────────────────────────────────┘
```

</div>

---

## 🤝 贡献指南

> 欢迎贡献代码！请先阅读 [AGENTS.md](./AGENTS.md) 了解项目的 Agent 配置规范。

---

## 📄 License

See [LICENSE.md](./LICENSE.md)

---

<p align="center">
  <sub>Built with ❤️ by <a href="https://anthropic.com">Anthropic</a></sub>
</p>