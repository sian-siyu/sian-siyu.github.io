---
title: Git Commits提交规范
date: 2025-04-01 10:24:09
tags:

---

> Conventional Commits 是一种用于 Git 提交信息格式化的约定，旨在使提交信息更加规范和一致，便于自动化工具进行处理和分析。

#### 提交信息格式

Conventional Commits 的基本格式如下：

```
<type>(<scope>): <subject>
```

- **type**：表示提交的类型，常见的类型包括：

| 值           | 描述                                                         |
| ------------ | ------------------------------------------------------------ |
| **feat**     | 新增一个功能（feature）                                      |
| **fix**      | 修复一个Bug                                                  |
| docs         | 文档变更、更新                                               |
| style        | 代码格式化（不影响功能，例如空格、分号等格式修正）           |
| **refactor** | 代码重构，不影响功能                                         |
| perf         | 改善性能                                                     |
| test         | 添加或更新测试                                               |
| build        | 变更项目构建或外部依赖（例如scopes: webpack、gulp、npm等）   |
| ci           | 更改持续集成软件的配置文件和package中的scripts命令，例如scopes: Travis, Circle等 |
| chore        | 变更构建流程或辅助工具                                       |
| **revert**   | 代码回退，回滚到之前的提交                                   |
- **scope**（可选）：表示提交影响的范围或模块，例如 `login`、`utils` 等。
- **subject**：简要描述提交的内容。

#### 示例

以下是使用 Conventional Commits 规范的一些示例：

- **引入新功能（feat）**：

  ```
  feat(user-module): 添加用户注册功能
  ```

- **修复 bug（fix）**：

  ```
  fix(auth): 修复登录验证逻辑错误
  ```

- **代码重构（refactor）**：

  ```
  refactor(api): 简化数据获取逻辑
  ```

- **文档更新（docs）**：

  ```
  docs(readme): 更新贡献指南
  ```

- **代码格式化（style）**：

  ```
  style(button): 统一按钮样式
  ```

- **测试（test）**：

  ```
  test(cart): 添加购物车功能测试用例
  ```