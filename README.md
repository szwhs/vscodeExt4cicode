# Citect Cicode（VS Code 扩展）

用于 VS Code 的 Citect Cicode 语法高亮与格式化扩展。
主要解决citect cicode 打开文件慢，没有代码折叠，代码分析和查找不方便的问题。

## 功能

- `.ci` 文件识别与语法高亮
- 文件列表与过滤：侧边栏提供 “Cicode 文件” 视图仅列出指定后缀文件；并提供命令一键切换 Explorer 仅显示指定后缀文件
- 代码片段（Snippets）：提供 `ci.if/ci.ife/ci.fori/ci.while/ci.whilet/ci.select/ci.func/ci.funcfull` 等常用模板（降低与自动补全冲突）
- 格式化：Tab 缩进 + 一行一语句（按 `;` 拆分）
- 注释保留：`//`、`!`、`/* ... */`
- 字符串高亮：双引号字符串，字符串内双引号使用 `""` 表示；反斜杠不作为通用转义（兼容 Windows 路径末尾 `\`）
- 支持从本地离线帮助自动提取保留关键字与系统函数，用于高亮

## 安装

- 方式 1：从 VSIX 安装
  1. 从 `releases/` 下载最新 `.vsix`
  2. VS Code 命令面板执行：`Extensions: Install from VSIX...`
  3. 选择下载的 `.vsix`，重载窗口

## 使用

- 打开 `.ci` 文件（语言会识别为 `Cicode`）
- 需要格式化时使用：`Format Document` / `Alt+Shift+F`
- 输入代码片段触发词并按 `Tab` 展开模板（详情见 `docs/snippets.md`）
- 只想专注查看指定后缀文件时：
  - 在资源管理器中查看 “Cicode 文件” 视图（默认仅列出 `.ci`）
  - 打开命令面板（`Ctrl+Shift+P`）：
    - 执行：`Cicode: 仅显示指定后缀文件（切换 Explorer）`：切换默认资源管理器过滤/恢复
    - 执行：`Cicode: 刷新 Cicode 文件视图`：刷新侧边栏的 “Cicode 文件” 列表

## 格式化规则

- 规则说明见：`docs/formatting-rules.md`
