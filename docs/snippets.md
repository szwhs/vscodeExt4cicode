# Cicode 代码片段（Snippets）

本扩展为 Cicode 提供常用代码片段，用于快速生成常见结构模板。

## 1. 使用方法

1. 在 VS Code 中打开 `.ci` 文件（语言为 `Cicode`）
2. 在编辑器里输入触发词
3. 按 `Tab`（或回车）展开模板
4. 使用 `Tab` 在占位符之间跳转，填写参数

## 2. 触发词列表

### 2.1 控制流

- `if`：简单 IF
- `ife`：IF / ELSE
- `select`：SELECT CASE
- `while`：WHILE 条件循环
- `whilet`：WHILE TRUE + SLEEP
- `fori`：FOR 循环

### 2.2 函数模板

- `func`：简单 FUNCTION
- `funcfull`：完整函数模板（示例：`PRIVATE` + `INT` + `FUNCTION` + 参数 + `RETURN`）

### 2.3 注释模板

- `file-header` / `@file-header`：文件头注释模板
- `function-header` / `@function-header`：函数注释模板

## 3. 常见问题

- 片段只会在 `.ci` 文件中生效：请确认右下角语言模式为 `Cicode`
- 若输入触发词没有提示：尝试重新加载窗口（`Developer: Reload Window`）或确认已安装/启用本扩展

