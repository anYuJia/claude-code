# Claude Code

[English](#english) | [中文](#中文)

---

## 中文

### 项目简介

Claude Code 是 Anthropic 推出的 AI 编程助手 CLI 工具，提供强大的代码编辑、任务自动化和智能辅助功能。本项目是 Claude Code 源码的恢复版本，通过 source map 逆向还原并补齐缺失模块后得到的完整源码树。

### 功能特性

- **智能代码编辑** - AI 驱动的代码补全、重构和建议
- **任务自动化** - 支持复杂的多步骤任务规划和执行
- **MCP 集成** - 完整的 Model Context Protocol 支持
- **会话管理** - 强大的会话历史和状态管理
- **权限系统** - 精细化的工具调用权限控制
- **调试能力** - 内置调试工具和日志系统

### 技术栈

| 分类 | 技术 |
|------|------|
| 语言 | TypeScript |
| 包管理 | Bun |
| 运行时 | Node.js 24+ |
| SDK | Anthropic SDK, Claude Agent SDK |
| 协议 | MCP (Model Context Protocol) |
| 监控 | OpenTelemetry |
| UI | React, Ink (CLI UI) |

### 环境要求

- **Bun**: 1.3.5 或更高版本
- **Node.js**: 24.0.0 或更高版本

### 快速开始

```bash
# 安装依赖
bun install

# 运行 CLI
bun run dev

# 查看版本
bun run version

# 查看帮助
bun run dev --help
```

### 项目结构

```
claude-code/
├── src/                    # 源代码
│   ├── bridge/            # 桥接层 (与外部通信)
│   ├── assistant/         # 助手核心逻辑
│   ├── bootstrap/         # 启动引导
│   ├── skills/            # 技能系统
│   └── ...
├── shims/                 # 兼容层 (native bindings)
├── vendor/                # 第三方源码
├── AGENTS.md              # Agent 配置
└── package.json
```

### 可用命令

```bash
# 开发模式运行
bun run dev

# 生产模式运行
bun start

# 查看版本信息
bun run version
```

### 贡献指南

欢迎贡献代码！请先阅读 [AGENTS.md](./AGENTS.md) 了解项目的 Agent 配置规范。

### License

详见 [LICENSE.md](./LICENSE.md)

---

## English

### Overview

Claude Code is an AI-powered programming assistant CLI tool developed by Anthropic, providing powerful code editing, task automation, and intelligent assistance. This project is a restored version of the Claude Code source code, reconstructed from source maps with missing modules backfilled.

### Features

- **Intelligent Code Editing** - AI-driven code completion, refactoring, and suggestions
- **Task Automation** - Support for complex multi-step task planning and execution
- **MCP Integration** - Complete Model Context Protocol support
- **Session Management** - Powerful session history and state management
- **Permission System** - Fine-grained tool call permission control
- **Debugging Capabilities** - Built-in debugging tools and logging system

### Tech Stack

| Category | Technology |
|----------|------------|
| Language | TypeScript |
| Package Manager | Bun |
| Runtime | Node.js 24+ |
| SDK | Anthropic SDK, Claude Agent SDK |
| Protocol | MCP (Model Context Protocol) |
| Monitoring | OpenTelemetry |
| UI | React, Ink (CLI UI) |

### Requirements

- **Bun**: 1.3.5 or higher
- **Node.js**: 24.0.0 or higher

### Quick Start

```bash
# Install dependencies
bun install

# Run CLI
bun run dev

# Check version
bun run version

# View help
bun run dev --help
```

### Project Structure

```
claude-code/
├── src/                    # Source code
│   ├── bridge/            # Bridge layer (external communication)
│   ├── assistant/         # Assistant core logic
│   ├── bootstrap/         # Bootstrap
│   ├── skills/            # Skills system
│   └── ...
├── shims/                 # Compatibility layer (native bindings)
├── vendor/                # Third-party source
├── AGENTS.md              # Agent configuration
└── package.json
```

### Available Commands

```bash
# Run in development mode
bun run dev

# Run in production mode
bun start

# View version information
bun run version
```

### Contributing

Contributions are welcome! Please read [AGENTS.md](./AGENTS.md) to understand the project's Agent configuration specifications.

### License

See [LICENSE.md](./LICENSE.md) for details.