# PicoClaw

PicoClaw 是一款超轻量级个人 AI 助手，支持多种 LLM 提供商，强调轻量、快速与安全。

## 应用信息

- 应用名：PicoClaw
- 包名：`picoclaw`
- 当前版本：`0.2.8`
- 发布者：EWEDL
- 上游项目：<https://github.com/sipeed/picoclaw>
- 问题反馈：<https://github.com/sipeed/picoclaw/issues>

## 简介

皮皮虾，超轻量级个人 AI 助手，支持多种 LLM 提供商，比小龙虾更小、更轻快、更安全。

## 安装说明

从 FnDepot 安装后即可使用。当前仓库内提供 `picoclaw.fpk` 安装包。

## 更新说明

#### 🚀 新特性 (New Features)
- CLI 与终端变更：新增自定义 OpenAI 兼容端点 CLI 支持，同时移除 TUI 界面
- MCP 增强：新增 MCP CLI 管理命令（show/add/list/remove/test/edit），新增 MCP 斜杠命令及工具详情展示
- 硬件与串口通信：新增跨平台串口硬件工具支持（已接入运行时框架和仪表盘）
- Web 前端：支持在 Web 界面直接下载文件

#### ✨ 体验优化与增强 (Enhancements)
- AI 思考与推理展示：统一各聊天渠道中 Reasoning 与 Tool Calls 的可见性，新增 Thought visibility 切换开关
- Prompt 与 Agent：引入结构化 Prompt 分层机制，并将工具 Prompt 迁移至 capability slots
- 配置管理：新增“配置保存并重启 Prompt”功能提示，支持在模型列表中明确指定 provider 字段
- 工具反馈：统一各聊天渠道和 Pico 端的工具反馈动画，并为聊天反馈提供独立消息模式

#### 🐛 核心修复 (Linux/通用相关)
- 系统与守护进程：修复 PID 文件单例检查，PID=1 视为过期进程（更友好于 Linux Systemd/Docker）
- 串口（Linux）：改进 Unix 系统下的串口操作取消机制和超时轮询逻辑
- 推理持久化：修复并持久化 DeepSeek 与 Web 聊天的 reasoning_content 至 SQLite
- 配置诊断：配置文件格式错误时提供精确诊断信息
- 第三方集成：修复 Telegram OAuth 链接保留问题、Feishu 图片下载降级兼容与发送图片支持
- Pico/工具调用：统一 tool_calls 与思考过程消息类型，修复 MCP 工具参数 null/空对象问题，优化 Web 搜索 fallback，修复 Cron 会话密钥传播防止工具重复响应

---
*上次更新：2026-05-04*
