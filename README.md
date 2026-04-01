# Claude Code 2.1.88 Source Recovery

<p align="center">
  <img src="https://img.shields.io/badge/Version-2.1.88-blue.svg" alt="Version">
  <img src="https://img.shields.io/badge/Status-Recovered-green.svg" alt="Status">
  <img src="https://img.shields.io/badge/Language-TypeScript-blue.svg" alt="Language">
  <img src="https://img.shields.io/badge/UI-Ink%20%2F%20React-orange.svg" alt="UI">
</p>


> [!IMPORTANT]
> **这是一个针对 `@anthropic-ai/claude-code` 2.1.88 版本的源码整理与重建项目。**
> 该版本发布到 npm 时附带了可还原源码的 source map。本项目基于 `sources` 和 `sourcesContent` 将其还原为可读的源码目录，旨在研究 Claude Code 的 CLI 架构、命令系统及 MCP 实现。

## 项目结构概览

本项目以 `src/` 为核心，高度还原了原始代码组织：

- **`src/entrypoints/`** - CLI 入口与初始化逻辑
- **`src/commands/`** - 强大的命令系统 (`login`, `mcp`, `review`, `tasks` 等)
- **`src/components/`** - 基于 **React + Ink** 的终端 UI 组件
- **`src/services/`** - 核心业务逻辑 (策略、同步、远程能力等)
- **`src/hooks/`** - 交互式终端状态管理
- **`src/utils/`** - 认证、文件操作、进程管理等工具函数
- **`src/ink/`** - 定制的终端渲染基础设施

---

## 源码亮点

从还原的代码中，我们可以深入探索以下核心设计：

- **命令装载机制**：支持内建命令、动态 skills、插件及 MCP 命令的混合装载。
- **终端 UI 艺术**：如何利用 React 组件在终端中构建复杂的交互界面。
- **MCP 深度集成**：Model Context Protocol 在 CLI 中的具体实现与应用。
- **Feature Flags**：源码中随处可见的特性裁剪与构建期控制逻辑。

---

## ⚠️ 免责声明

- **非官方项目**：本仓库并非 Anthropic 官方仓库，亦不代表其立场。
- **版权说明**：原始代码的版权、商标及相关权利归原权利方（Anthropic）所有。
- **研究用途**：本项目仅供归档、结构分析与源码阅读，不应被视为官方开源项目。
- **法律风险**：如需二次发布或商用，请自行评估相关许可与法律风险。

---

## 后续计划 (待补齐)

补充运行依赖
添加claude code学习路线

---

## 致谢

感谢发布时未移除的 **Source Map**的同志，让这份精致的工程结构得以重现。

---

## Star History

[![Star History Chart](https://api.star-history.com/image?repos=wy66064628/CrazyCodePulse&type=date&legend=top-left)](https://www.star-history.com/?repos=wy66064628%2FCrazyCodePulse&type=date&legend=top-left)
