# Lingstyle Design

Lingstyle 可视化设计器插件，版本 0.1.0。

## 安装

需要 Node.js 22.12+，以及支持本地 MCP 服务、MCP Apps 和 thread entrypoint 的 Codex 客户端。

在客户端的插件市场中添加此 Git 仓库：

https://github.com/mybricks/lingstyle-design-codex-plugin-package.git

也可以通过 CLI 添加市场：

```sh
codex plugin marketplace add https://github.com/mybricks/lingstyle-design-codex-plugin-package.git
```

然后在插件目录中选择 Lingstyle Design 市场，安装并启用 Lingstyle Design。
在对话中输入“打开 Lingstyle 面板”。无需安装 npm 依赖或启动开发服务器。

## 更新产物

本仓库由 lingstyle-design-codex-plugin 源码仓库的 `pnpm package:codex:git` 生成。
请在源码仓库修改后重新打包，再提交并推送此仓库。
