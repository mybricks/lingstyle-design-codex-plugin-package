# Lingstyle Design Codex 插件

为 Codex 提供可视化设计器、项目管理和虚拟项目文件编辑能力。本仓库是预编译插件产物，包含 MCP 服务、前端和 designer skill，无需安装 npm 依赖或启动 Vite。

## 通过 Git 安装

需要 Node.js 22.12+ 和支持插件及 MCP Apps 的 Codex 客户端。

将下面内容发给 Codex：

```text
请通过 Git marketplace 安装 Lingstyle Design 插件：
先运行 codex plugin marketplace add mybricks/lingstyle-design-codex-plugin-package，
再运行 codex plugin add lingstyle-design@lingstyle-design-git，
最后运行 codex plugin list 确认插件已启用。
发布仓库已包含编译产物，无需执行 npm install。
安装完成后提醒我完全退出并重新启动 Codex，并介绍插件功能和使用方式。
```

手动安装及更新见 [Codex 安装指南](CODEX.INSTALL.md)。

## 使用

安装并重启 Codex 后，在对话中引用 Lingstyle Design 插件，或说“打开 Lingstyle 面板”。在应用首页创建或打开项目，进入设计器后可让 Codex 读取、创建、修改或删除虚拟项目中的文件。

项目默认保存在本机 `~/.lingstyle-design/projects/`，独立于插件安装目录。可通过 MCP 环境变量 `LINGSTYLE_DATA_DIR` 指定存储位置。

## 发布内容

- `.agents/plugins/marketplace.json`：Git marketplace 清单。
- `.codex-plugin/plugin.json`：插件清单。
- `.mcp.json`：MCP 服务配置。
- `skills/designer/`：设计器技能及编码规范。
- `dist/server.mjs`：已内嵌依赖的 MCP 服务。
- `dist/panel.html`：已内嵌前端资源的应用页面。

版本：0.1.0。请在源码仓库运行 `pnpm package:codex` 更新产物，然后提交并推送本仓库。
