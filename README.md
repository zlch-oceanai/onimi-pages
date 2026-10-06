# Onimi Pages & Slides

One `onimi-pages` Skill to create and continue Pages or editable Slides in your Agent,
preview and validate the result, then save private drafts or publish when requested.
Local creation needs no account. Cloud operations use the existing `onimi-pages` MCP
connection and the connected account's actual permissions.

**English** · [简体中文](docs/zh-CN/README.md)

## Install and use

The official source repository is https://github.com/zlch-oceanai/onimi-pages.
If that repository is publicly available, use the current Agent's supported plugin
import or Skill installation route. A Skill installation alone does not register an
MCP server on every host. Read the bundled
[installation guide](skills/onimi-pages/references/installation.md) for connection help.

For a client supported by the Skills CLI:

```sh
npx --registry=https://registry.npmjs.org skills@1.5.26 add zlch-oceanai/onimi-pages --skill onimi-pages --global --agent codex
```

This example targets Codex explicitly. For another Agent, replace `codex` with
that client's supported Skills CLI identifier, such as `claude-code` or `cursor`.
Target only the current Agent. Preserve any existing folder and local changes.
If old Creator/Publish folders are active, follow the
[migration guide](skills/onimi-pages/references/migration.md) before adding another
entrypoint; do not assume a registry-owned installation can be replaced by a direct
manager. Host and registry installations retain their native update ownership.

Try: “Make a Page for my weekly review and preview it locally.” Or: “Continue my
selected Slides draft without publishing.” Read the
[Skill](skills/onimi-pages/SKILL.md) for the task-specific guidance.
Creating or saving a draft does not publish it; publishing does not automatically
make it public. When account access is needed, reuse an applicable connection or
approve browser OAuth yourself. Never provide a token in chat.

## Source and availability

This repository contains root portable `plugin.json` and `mcp.json`, a square icon,
MIT-0 license and the allowlisted single Skill. It contains no application code,
credentials, user content, npm package/lifecycle installer, direct-download receipt
or update manager, or public stable-channel archives.

Version 0.3.2 is a source candidate. GitHub hosting does not publish npm, promote
the direct stable manifest, or prove production client acceptance. The Codex plugin
submission remains incomplete until its dedicated reviewer account, five positive
and three negative real client cases, recording and portal checks are ready.
No fabricated video URL or account credentials are in this source.

The same portable source can be packaged for review using the application-owned
builder. The plugin host owns installed copies and their updates; review artifacts
and private submission evidence stay outside this repository.

[Website](https://onimi.ai) · [Help](https://onimi.ai/en/help) ·
[Privacy](https://onimi.ai/en/privacy) · [Terms](https://onimi.ai/en/terms)
