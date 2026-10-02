<div align="center">

# AutoDeploymentModel

### 让本地大模型从"能跑"到"能用"

[![Website](https://img.shields.io/badge/Website-adm.tuduoduo.top-2f81f7?style=flat-square)](https://adm.tuduoduo.top/)
[![ADM](https://img.shields.io/badge/ADM-v0.x-42a5f5?style=flat-square)](https://github.com/autoDeploymentModel/adm/releases)
[![License](https://img.shields.io/badge/license-see%20repos-lightgrey?style=flat-square)](#)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-42a5f5?style=flat-square)](#)

**ADM（Auto Deploy Model）** —— 把 llama.cpp 复杂的命令行启动指令装进一个图形界面，
本地下载、启动、对话、管理大模型，并内置 Agent 终端，把本地模型直接接入智能体工作流。

[🌐 官网](https://adm.tuduoduo.top/) ·
[📥 下载发布版](https://github.com/autoDeploymentModel/adm/releases) ·
[📖 文档](https://github.com/autoDeploymentModel/adm#readme) ·
[🐛 反馈问题](https://github.com/autoDeploymentModel/adm/issues)

</div>

---

## 项目一览

<table>
  <thead>
    <tr>
      <th width="26%">项目</th>
      <th width="46%">说明</th>
      <th width="28%">技术栈</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://github.com/autoDeploymentModel/adm"><b>ADM</b></a><br><sub>主项目 · 桌面端</sub></td>
      <td>本地大模型一键部署与管理：模型下载 / 启动 / 对话 / 可视化调参，内置 Agent 终端把本地模型接入智能体工作流</td>
      <td>Tauri 2 · Rust · 原生 ES 模块前端</td>
    </tr>
    <tr>
      <td><a href="https://github.com/autoDeploymentModel/adm-be"><b>ADM-BE</b></a><br><sub>DGX Spark 专用版</sub></td>
      <td>面向 NVIDIA DGX Spark 的大模型部署与管理桌面应用</td>
      <td>Rust · Tauri</td>
    </tr>
    <tr>
      <td><a href="https://github.com/autoDeploymentModel/hybrid-desktop-frontend"><b>hybrid-desktop-frontend</b></a><br><sub>可复用前端框架 Skill</sub></td>
      <td>从 ADM 桌面端抽离的零框架前端骨架，同一套代码可跑在 Tauri 2 / Wails v3 / Electron 等混合开发框架上</td>
      <td>原生 HTML / CSS / ESM</td>
    </tr>
    <tr>
      <td><a href="https://github.com/autoDeploymentModel/adm-binaries"><b>adm-binaries</b></a><br><sub>构建产物仓库</sub></td>
      <td>ADM 桌面端内置的 admAgent 二进制分发仓库，由构建流程自动同步</td>
      <td>Go · 自动分发</td>
    </tr>
  </tbody>
</table>

> `llamacpp` / `i-have-adhd` 等为上游 fork 或实验仓库，不在主页展示。

---

## ADM 能做什么

- **零命令行部署** —— 搜模型、下载（断点续传 + 国内镜像加速）、启动、打开 WebUI，全程图形化
- **内置 Agent 终端** —— 在应用内直接用本地模型驱动智能体：读写文件、跑命令、调 LSP/MCP/skills
- **模型即服务** —— 兼容 OpenAI 格式接口，可被其它工具复用
- **跨平台** —— Windows / macOS / Linux 一套代码

## 快速开始

```bash
# 桌面端（需 Node.js + pnpm + Rust 工具链）
pnpm tauri dev

# admAgent 服务端 / TUI（在 admAgent/ 目录内）
go build ./...
```

完整构建与发布说明见 [ADM 仓库 README](https://github.com/autoDeploymentModel/adm)。

## 加入我们

欢迎提 Issue、提 PR 或贡献代码 —— 先看看 [贡献指南](https://github.com/autoDeploymentModel/adm#readme) 与各仓库的 `AGENTS.md`。

<div align="center">
  <sub>AutoDeploymentModel · 让本地大模型用起来</sub>
</div>
