# Harness Engineering

## 课程简介

- 来源：walkinglabs 开源社区课程（[课程网站](https://walkinglabs.github.io/learn-harness-engineering/zh/)），非高校学分课程，以短讲形式发布
- 先修要求：有一个真实的代码仓库、熟悉 Git 与命令行、至少用过一款编码 Agent（如 Claude Code、Codex）
- 编程语言：不限，课程主体是仓库内的指令文件、配置与验证命令，可能涉及少量 Shell 或 Python 编写验证钩子
- 课程难度：🌟🌟
- 预计学时：约 12 讲，8 小时左右看课，另需至少 15 小时在自己的项目上实践

<!-- 用一两段话介绍这门课程，内容包括但不限于：
    （1）课程覆盖的知识点范围
    （2）与同类课程相比它的优势与特点
    （3）学习这门课程的体验与感受
    （4）自学这门课的注意点（踩过的坑、难度预警等等）
    （5）... ...
-->

这门课讨论的是一个很朴素的问题：模型的能力强，不等于它在你的仓库里干活可靠。"harness"这个词在 AI coding agent 的圈子里被用得越来越多了，但大部分人说 harness 的时候，其实指的是一个 prompt 文件。一个 prompt 文件不是 harness。

这节课要给 harness 一个精确的、可操作的定义。不是学术论文里的抽象概念，而是你今天就能拿去用的框架。harness 由五个子系统组成：指令、工具、环境、状态、反馈。每个子系统都有明确的职责和评判标准。

Learn Harness Engineering 是一门专注于 AI 编程智能体工程化落地的课程。通过系统的环境设计、状态管理、验证与控制机制，本课程旨在帮助你让 Codex 和 Claude Code 等 AI Agent 能够真正可靠地完成真实工程任务。它通过明确的规则和边界约束你的 AI 编程助手，帮助你更可靠地构建功能、修复 Bug 并自动化开发任务。

自学的第一个坑是缺少真实项目。没有仓库可折腾时，这门课会迅速退化成概念背诵，建议挑一个自己正在维护、有一定复杂度、需要跑测试的项目作为练习场。第二个坑是过度工程：一开始就想搭出一套完美的 harness，结果配置文件越写越多、验证命令没人维护，反而增加了负担。原课程强调的“先让它可靠，再让它优雅”，从最小可用的验证回路开始更现实。第三个坑是把二手解读当成课程结论。Harness Engineering 是近年热起来的概念，译名和术语尚未统一，各类解读常有夸张成分，遇到关键论断建议回到原始讲次和 OpenAI 的 harness engineering 文章核对。

## 课程资源

- 课程网站：<https://walkinglabs.github.io/learn-harness-engineering/zh/>

## 资源汇总

[github官方仓库](https://github.com/walkinglabs/learn-harness-engineering/tree/main)