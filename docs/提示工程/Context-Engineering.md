# 上下文工程

## 课程简介

- 来源：davidkimai 发起的开源课程 Context-Engineering（[课程网站](https://deepwiki.com/davidkimai/Context-Engineering)），原始内容托管在 [GitHub 仓库](https://github.com/davidkimai/Context-Engineering)
- 先修要求：熟悉提示工程基础（零样本、少样本、链式思考），会写 Python 并调用过至少一种 LLM API；涉及记忆、RAG、Agent 的章节需要理解向量检索与工具调用的基本概念
- 编程语言：Python，讲义中的示例以 Notebook 风格的单文件脚本提供，配置文件使用 YAML
- 课程难度：🌟🌟🌟🌟
- 预计学时：课程自述为 12 周的分阶段学习路径，按每周 4 至 6 小时估算约 50 至 70 小时；若只读基础与系统实现两部分，20 小时左右可完成第一遍

课程的核心命题是：提示工程只解决“你说什么”，上下文工程解决“模型看到的其他一切”。作者引用 Karpathy 的定义——上下文工程是“把刚刚好的信息填进上下文窗口的细腻艺术”，并采用 A Survey of Context Engineering（综述 1400 余篇论文）的界定：上下文不只是用户发出去的那段提示词，而是推理时刻提供给模型的完整信息载荷，涵盖示例、记忆、检索结果、工具、状态与控制流。课程用一套生物学隐喻搭起递进的四级结构：原子（单条指令与简单约束）、分子（少样本示例与演示集）、细胞（持久记忆、状态管理、上下文窗口）、器官（多步流程、专家分工、系统编排），之上是神经系统与语义场（推理框架、验证工具、认知模式、吸引子与共振），再到协议壳与统一系统，最后是元递归框架（自我反思、递归改进、可解释演化）。每个层级都对应现实中的技术形态，从基础提示工程一路映射到多 Agent 系统与自组织系统。

相较同类材料，它最鲜明的特点是把上下文当成一个可以“度量、删减、编排”的工程对象，而不是一堆提示技巧的集合。课程给出六条明确的方法论：从第一性原理出发、只补模型确实缺失的部分、对 token 成本与延迟与质量分数全部量化、删除优于堆砌、代码优于幻灯片（每个概念都有可运行单元）、一切都要可视化（ASCII 图与符号图贯穿全篇）。同时它把最新研究直接嵌进教材，例如 MEM1 的记忆与推理合并、IBM Zurich 的认知工具（把结构化提示模板当工具调用，使 GPT-4.1 在 AIME2024 上 pass@1 从 26.7% 提升到 43.3%）、ICML Princeton 关于涌现符号机制的三段式注意力结构，这些论文被用来解释为什么 Markdown、JSON 这类结构化格式更利于模型解析。

## 课程资源

- [课程网站](https://deepwiki.com/davidkimai/Context-Engineering)，原始讲义见 [GitHub 仓库](https://github.com/davidkimai/Context-Engineering)
- 课程教材：一份 [Context Engineering 综述](https://arxiv.org/pdf/2507.13334) 作为理论参考

## 资源汇总

[官方 GitHub 仓库](https://github.com/davidkimai/Context-Engineering) 汇总了全部讲义、模板、示例项目、Agent 命令与论文引用