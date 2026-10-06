# Onimi Pages & Slides

在自己的 Agent 中用唯一的 `onimi-pages` Skill 创作和继续修改网页或可编辑演示文稿，
预览、校验结果，再按需要保存私有草稿，或在明确要求时发布。本地创作不需要账号；
云端操作复用原有 `onimi-pages` MCP 连接，并遵守已连接账号的实际权限。

[English](../../README.md) · **简体中文**

## 安装与使用

官方源码仓库：https://github.com/zlch-oceanai/onimi-pages。
仓库公开可用后，使用当前 Agent 支持的插件导入或 Skill 安装方式。
安装 Skill 不代表每个宿主都已注册 MCP，连接步骤见安装包内
[安装指南](../../skills/onimi-pages/references/installation.zh-CN.md)。

支持 Skills CLI 的客户端可以使用：

```sh
npx --registry=https://registry.npmjs.org skills@1.5.26 add zlch-oceanai/onimi-pages --skill onimi-pages --global --agent codex
```

该示例明确指定 Codex。使用其他 Agent 时，把 `codex` 换成该客户端受 Skills CLI
支持的实际标识，例如 `claude-code` 或 `cursor`。只指定当前 Agent，保留已有目录与个人修改。
发现旧 Creator/Publish 活跃目录时，
先按[迁移指南](../../skills/onimi-pages/references/migration.md)处理，避免多个入口同时生效；
不能假定直接下载 manager 可以替换宿主管理的安装。各宿主和注册渠道仍负责自己的更新。

可以试：“做一个周报网页，在本地预览。”或者：“继续修改我选定的 Slides 草稿，暂不发布。”
按任务读取[Skill 指引](../../skills/onimi-pages/SKILL.md)。创作或保存草稿不代表发布，
发布也不自动公开。需要账号权限时复用适用连接，或者由你亲自批准浏览器 OAuth；
不要在聊天中提供 Token。

## 源码与可用状态

本仓库仅包含根目录 portable `plugin.json`、`mcp.json`、方形图标、MIT-0 许可和
经审核允许分发的唯一 Skill，不含应用代码、凭据、用户内容、npm 包或安装器、
直接下载收据与更新 manager，也不包含公共 stable 渠道归档。

0.3.2 是源码候选版本。GitHub 托管不会发布 npm、推广直接下载稳定清单，
也不能证明生产客户端验收。Codex 插件提交仍需专用审核账号、五个正向与三个负向
真实客户端案例、真实录屏和门户检查；源码中没有编造的视频地址或账号凭据。

这些 portable 源码由应用侧构建器打包审阅。插件宿主负责安装副本和更新，
审阅产物与私有提交证据留在本仓库之外。

[网站](https://onimi.ai) · [帮助](https://onimi.ai/zh-CN/help) ·
[隐私](https://onimi.ai/zh-CN/privacy) · [服务条款](https://onimi.ai/zh-CN/terms)
