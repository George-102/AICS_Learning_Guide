# TOOL-101：Learning Git Branching

## 课程简介

- 来源：Learn Git Branching 开源互动教程（[课程网站](https://learngitbranching.js.org/?locale=zh_CN)），以浏览器内可视化沙盒的形式发布
- 先修要求：无需任何 Git 或图形化客户端经验；能使用命令行（知道 `cd`、`ls` 等基础命令）即可，了解“版本控制”大致是用来保存历史版本的即可
- 编程语言：无，学习者通过输入 Git 命令完成关卡
- 课程难度：🌟
- 预计学时：主线与远程仓库两部分约 8 小时，全部通读并完成挑战关约 15 小时

它把 Git 的分支操作变成可玩的关卡。教程围绕几个核心关卡组展开：基础篇讲 `commit`、`branch`、`merge`、`rebase`，进阶篇讲在提交之间移动的 `checkout`、`reset`、`revert`、`cherry-pick` 与交互式 `rebase`，然后是“移动提交记录”“杂项”“高级话题”等组，最后是远程仓库部分，覆盖 `clone`、`fetch`、`pull`、`push`、跟踪分支与远程分支。每个关卡只有一个明确目标，右侧是可视化仓库图，你输入命令后提交节点与分支指针会立即移动，目标达成即通关，进度保存在浏览器本地。

它最大的优势是把抽象的分支模型直接变成图像。Git 最令人困惑的地方在于“提交是节点、分支是指针、HEAD 是当前位置”这套心智模型，讲义里写十遍也不如亲手用 `git rebase` 把游离的提交贴到另一条分支上、看着节点在图中重排来得直观。其次，每一个关卡都是先演示再练习，左侧有简短说明与命令提示，右侧随时可以用 `undo` 和 `reset` 撤销，失败零成本，因此可以放心大胆地试错，这在真实仓库里不可能做到。相较于《Pro Git》这类系统教材，它不逐项讲解原理与配置；相较于零散的 Git 速查表，它又提供了循序渐进的顺序和即时反馈。

## 课程资源

- 课程网站：<https://learngitbranching.js.org/?locale=zh_CN>
- 课程教材：可以配合《Pro Git》（[中文版在线免费](https://git-scm.com/book/zh/v2)）补充原理与配置

## 资源汇总

[官方 GitHub 仓库](https://github.com/pcottle/learnGitBranching)