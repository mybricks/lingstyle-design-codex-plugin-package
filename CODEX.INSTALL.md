# 安装 Lingstyle Design

需要 Node.js 22.12+ 和 Codex CLI。

```sh
codex plugin marketplace add mybricks/lingstyle-design-codex-plugin-package
codex plugin add lingstyle-design@lingstyle-design-git
codex plugin list
```

已注册 marketplace 时可跳过第一步。更新：

```sh
codex plugin marketplace upgrade lingstyle-design-git
```

安装或更新后，完全退出并重新启动 Codex，加载 skill 和 MCP 服务。默认使用远端默认分支，也可在 marketplace add 命令后添加 `--ref <分支名>`。

无需在插件目录执行 npm install。打开可视化设计器需要客户端支持 MCP Apps 和 thread entrypoint。

重启后引用 Lingstyle Design 插件，或发送“打开 Lingstyle 面板”，再在应用中创建或打开项目。可让 Codex 编辑设计器中的虚拟项目文件。
