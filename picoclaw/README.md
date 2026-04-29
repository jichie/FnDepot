# PicoClaw

PicoClaw 是一款超轻量级个人 AI 助手，支持多种 LLM 提供商，强调轻量、快速与安全。

## 应用信息

- 应用名：PicoClaw
- 包名：`picoclaw`
- 当前版本：`0.2.7`
- 发布者：EWEDL
- 上游项目：<https://github.com/sipeed/picoclaw>
- 问题反馈：<https://github.com/sipeed/picoclaw/issues>

## 简介

皮皮虾，超轻量级个人 AI 助手，支持多种 LLM 提供商，比小龙虾更小、更轻快、更安全。

## 安装说明

从 FnDepot 安装后即可使用。当前仓库内提供 `picoclaw.fpk` 安装包。

## 更新说明

#### 鉴权流程调整（重点）
- 🔐 **移除环境变量令牌配置** - 不再要求设置 `PICOCLAW_LAUNCHER_TOKEN`
- 🔐 **改为官方密码初始化流程** - 首次打开 Web 控制台时按弹窗设置登录密码

#### Web/Gateway 稳定性
- ✅ **增强 Launcher/Gateway 多主机绑定能力** - 改进 Host 规范化处理
- ✅ **优化代理场景下 WebUI 与 WebSocket 连接稳定性** - 提升复杂网络环境可用性
- ✅ **包含网络容错与会话路由相关修复** - 降低连接异常和中断概率

#### 功能与通用更新
- 🔎 **新增可配置搜狗搜索** - 并支持按界面语言自动切换
- 🧰 **包含多项通用稳定性修复** - 持续提升 Linux 运行体验

---
*上次更新：2026-04-29*
