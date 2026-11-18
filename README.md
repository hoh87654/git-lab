# git-lab

Git 与 GitHub 的练习仓库：完整走一遍 **克隆 → 提交 → 分支 → 推送 → Pull Request → 合并**。

## 这是什么

一个只含文档和一个 Python 小脚本的练习仓库，用于熟悉 Git 工作流，不含业务代码。

## 怎么运行

```bash
python3 hello.py
```

输出：

```
Hello, Git!
```

## 目录结构

| 路径 | 说明 |
|---|---|
| `hello.py` | 最小可运行示例 |
| `docs/index.html` | GitHub Pages 静态页 |
| `.github/` | Issue 与 PR 模板 |

## 学习笔记

- **提交（commit）** 是快照，不是差异；每次提交都能回到当时的完整状态
- **分支（branch）** 是指向某个提交的可移动指针，用来隔离未完成的改动
- **推送前先拉取**，避免 `! [rejected] ... fetch first`

## 为什么单独开分支

主干（main）永远保持可运行；没把握的改动放分支里折腾，坏了直接删，不影响别人。
合并时用 PR，多一次「合并前看 diff」的机会。
