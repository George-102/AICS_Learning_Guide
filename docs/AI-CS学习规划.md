# 一份仅供参考的学习规划

本指南旨在构建一套面向 AI 时代的计算机科学学习体系，帮助计算机专业初学者建立系统的知识结构，掌握现代软件工程与 AI 应用开发能力，并找到适合自己的专业发展方向。

这份指南并非要求所有学习者按照固定顺序完成全部课程。你可以根据自己的知识基础、学习阶段和发展目标，选择适合自己的学习路径。

## 工具和技能

> *_工欲善其事，必先利其器。_*

工具和技能是学校很少教授的东西，但却是提升工作学习效率的必备。

| 工具或技能           | 说明                                                         |
| :------------------- | :----------------------------------------------------------- |
| 学会提问             | **学会提问**，如果你刚接触到这个专业，你可能根本不会正确提问，遇到问题先问AI，使用搜索引擎，直到最后再去麻烦别人，这里推荐阅读[提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/main/README-zh_CN.md)这篇文章，学会真正的提问方式。 |
| 魔法（科学上网）     | 由于一些众所周知的原因，谷歌、GitHub 等网站在大陆无法访问，这也导致我们无法获得一些需要的资源，这时候就需要使用一点点**魔法**（科学上网）。 |
| shell                | 命令行（shell）是一门被忽略的技能，但实际上，它会极大地提高你作为工程师的灵活性以及生产力，[命令行的艺术](https://github.com/jlevy/the-art-of-command-line/blob/master/README-zh.md)是一份非常经典的教程，强烈推荐大家掌握一些基本的shell命令。 |
| 开发环境和编辑器     | 开发环境是程序员工作的必备环境，如果你是 Mac 用户，那么你很幸运，这份[指南](https://sourabhbajaj.com/mac-setup/) 将会手把手地带你搭建起整套开发环境。如果你是 Windows 用户，在开源社区的努力下，你同样可以获得与其他平台类似的体验：[Scoop](https://github.com/ScoopInstaller/Scoop/wiki/Quick-Start)。现如今我们更多的是使用Visual Studio这样的集成开发环境，其中最著名的是[VS Code](https://github.com/viatsko/awesome-vscode)，在VS Code中，我们可以使用各种插件配置一个好的开发环境提升我们的开发效率。 |
| 编程语言的开发工具链 | 编译器、包管理、依赖与构建工具。尽管如今的IDE已经有很强大的功能，能够一键打包运行代码，但是某些情况下（例如了解代码构建原理，或是追求极致的构建效率）我们仍然需要使用编程语言的开发工具链，例如GNU Make是一款工程构建工具，善用 GNU Make 会让你养成代码模块化的习惯，同时也能让你熟悉一些大型工程的编译链接流程。 |
| Git                  | 版本控制、分支合并、PR 与协作流程。一款代码版本控制工具。Git一定是每个学 CS 的童鞋必须掌握的神器之一。 |
| Markdown             | 编写 README、笔记与技术文档。计算机行业最常用的文档格式，学会后你便拥有极致的编排文档的能力。 |
| Docker               | 容器化开发环境与镜像部署。一款相较于虚拟机更轻量级的软件打包与环境部署工具。 |
| Vim/Emacs            | 高效终端编辑器与远程开发。Vim是一款命令行编辑工具，它能够极大地提高你的开发效率；Emacs是与 Vim 齐名的经典编辑器，同样具有极高的开发效率，同时具有更为强大的扩展性。 |
| Latex                | 学术论文与规范化文档排版。~~逼格提升~~ 论文排版工具。        |

## 计算机科学基础

> _九层之台，起于累土。_

计算机科学基础是所有上层能力的共同地基，也是 AI 最难替你补上的部分。代码可以生成，但对原理的理解不能外包：遇到性能瓶颈、诡异的并发问题或者线上故障时，能救你的恰恰是操作系统、网络、数据结构这些“老知识”。建议先广后深，下面每门课都附了该领域的经典课程与教材，不必全部学完，选一条适合自己的线路走通即可。

| 课程                   | 说明                                                         |
| :--------------------- | :----------------------------------------------------------- |
| 数学基础               | 微积分、线性代数、离散数学。**数学决定了你在这一行能走多远**：微积分是理解梯度与优化的入口，线代是所有机器学习和图形学的语言，离散数学则是算法、密码学与编译理论的共同底座。建议在大一就把微积分和线代学到“刻骨铭心”的程度，而不是考完就忘，如果课上讲得晦涩，可以参考 [MIT 18.06](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/) 的公开课程，以及 [3Blue1Brown](https://www.youtube.com/@3blue1brown) 那些把数学本质讲得极具美感的动画视频。 |
| 程序设计基础           | C/C++、Java、Python。编程语言是工具，重要的是理解语言背后的设计思想：数组、字符串、指针、面向对象。初学者不要同时学好几门语言，先深入一门，再通过第二门理解不同的编程范式与生态，会比“每门都学过一点”走得更远。 |
| 数据结构和算法         | 算法是计算机科学的核心，是**面试和刷题**绕不开的内容，也是几乎一切专业课程的基础。如何将实际问题通过数学抽象转化为算法问题，并选用合适的数据结构在时间和内存大小的限制下将其解决是算法课的永恒主题。零基础入门可先用《Hello 算法》建立直观理解，详见 [ALGO-101：Hello 算法](数据结构和算法/hello-algo.md)。 |
| 数字逻辑与计算机组成   | 逻辑电路、CPU、指令与存储层次。这一块回答一个朴素的问题：**程序到底是怎么跑起来的**。想要既有趣又完整地建立这套认知，很推荐从零开始造一台计算机的 [Nand2Tetris](https://www.nand2tetris.org/) 入门，再深入 [UCB CS61C](https://cs61c.org/) 这类体系结构课程。 |
| 操作系统               | 操作系统把复杂而混乱的硬件虚拟成一套优雅的抽象，是**所有应用的共同底座**。这门课真正的收获往往来自动手，没有什么比亲手写一个内核更能加深理解，这里推荐[MIT 6.S081 (基于 xv6)](https://pdos.csail.mit.edu/6.828/2021/index.html)以及[仓库](https://github.com/wlmrh/MIT-6.S081)来学习。 |
| 计算机网络             | 大名鼎鼎的 [Stanford CS144: Computer Network](https://cs144.github.io/)，8 个 Project 带你实现整个 TCP/IP 协议栈。如果你只是想在理论上对计算机网络有所了解，那么推荐阅读 [UCB CS168](https://sp25.cs168.io/) 这门课程配套的[教材](https://textbook.cs168.io/)。 |
| 数据库系统             | CMU 的著名数据库神课 [CMU 15-445: Introduction to Database System](https://15445.courses.cs.cmu.edu/spring2023/schedule.html) 会通过 4 个 Project 带你为一个用于教学的关系型数据库 [bustub](https://github.com/cmu-db/bustub) 添加各种功能。实验的评测框架也免费开源了，非常适合大家自学。此外课程实验会用到 C++11 的众多新特性，也是一个锻炼 C++ 代码能力的好机会。 |
| 编译原理与程序语言     | 理论学习推荐阅读大名鼎鼎的《龙书》。当然动手实践才是掌握编译原理最好的方式，推荐[北京大学编译原理实践](https://pku-minic.github.io/online-doc/#/)课程，丰富的实验配套和循序渐进的文档带你实现一个类C语言到 RISC-V 汇编的编译器。当然编译原理课程目录下也有众多其他优质实验供你选择。 |
| 软件工程               | 一份“能跑”的代码，和一份高质量的工业级代码是有本质区别的。我推荐的是伯克利的 [UCB CS169: software engineering](http://www.saasbook.info/courses)。但需要提醒的是，和大多学校（包括贵校）的软件工程课程不同，这门课不会涉及传统的 **design and document** 模式，即强调各种类图、流程图及文档设计，而是采用近些年流行起来的小团队快速迭代 **Agile Development** 开发模式以及利用云平台的 **Software as a service** 服务模式。 |
| 计算理论与人工智能基础 | 可计算性、复杂度、AI 与机器学习基础。这一部分偏理论，但它给你的是**边界感**：哪些问题根本上算不出来，哪些问题算得出来但代价高到不可接受，为什么有些优化注定徒劳。同时它也是理解现代 AI 的起点，帮助你看清传统人工智能、机器学习与深度学习之间的关系与差异，避免在技术热潮里只记得工具名字，却说不清它们解决了什么。 |

## AI 时代工程能力

> _君子生非异也，善假于物也。_

这一节与传统培养方案差别最大，但不意味着可以跳过基础。课程分两条线：一条用 AI 提效，写代码、查 bug、读源码都更快；另一条用 AI 造东西，把模型、检索与工具调用组合成可用的应用。Prompt 谁都能写，难的是让系统稳定、可评估、可监控、成本可控。

| 课程                                    | 说明                                                         |
| :-------------------------------------- | :----------------------------------------------------------- |
| AI 与 LLM 基础                          | 模型原理、Token、Embedding、能力边界。推荐卡帕西（Karpathy）的 [Neural Networks: Zero to Hero](https://karpathy.ai/zero-to-hero.html) 从零手写 GPT，以及 [《动手学深度学习》](https://zh.d2l.ai/)。 |
| 提示工程                                | 指令设计、结构化输出、工具调用与提示评估。推荐读读 [《提示工程指南》](https://www.promptingguide.ai/zh)，再用一批测试样本对比效果。 |
| AI 辅助学习                             | 用 AI 阅读教材、源码与论文，并独立核验与验证。让 AI 解释、追问反例、自己动手验证，避免“好像懂了”的错觉。 |
| AI 辅助软件开发                         | AI 编程工具、Agent 驱动的软件开发、工程化方法。可从 [Claude Code](https://www.anthropic.com/claude-code)、[Codex](https://openai.com/codex/)、[DeepSeek Harness](https://www.deepseek.com/en/harness/)入手。 |
| AI 辅助软件工程                         | 需求、设计、测试、审查、迁移与 CI/CD。把 AI 放进整个软件生命周期，而不只是敲代码那一步。 |
| 大模型应用开发                          | LLM API、流式输出、结构化响应、RAG 与 Agent 应用。入门推荐跟着 [Anthropic 的课程](https://github.com/anthropics/courses) 逐行跑一遍示例。 |
| 检索增强生成与知识工程                  | 文档切分、检索、重排、RAG 评估与 GraphRAG。动手搭一套文档问答，并用评估数据集验证检索效果，可参考 [LlamaIndex](https://docs.llamaindex.ai/)。 |
| 智能体工程                              | 规划、工具调用、记忆、多 Agent 与安全部署。推荐阅读 [Building Effective Agents](https://www.anthropic.com/research/building-effective-agents)。 |
| AI 评估与可观测性                       | 评估数据集、LLM 评审、Tracing 与错误分析。没有评估就无法判断改动好坏，工具可看 [Ragas](https://docs.ragas.io/) 与 [Langfuse](https://langfuse.com/)。 |
| AI 应用部署工程                         | 服务部署、并发流式、监控、成本与模型回滚。最快的成长方式是把小项目真正部署上线并交给别人使用。 |

## 专业方向

> _闻道有先后，术业有专攻。_

没有人在本科阶段能把所有方向学一遍，也不必如此。建议以兴趣、科研目标和就业规划的交集为准，选定一到两个方向持续深入。入门标准很朴素：能读懂经典论文、能复现一个小实验、能说清该方向的核心问题与权衡。暂时没想清楚也不要焦虑，把基础打扎实，大多数方向的大门都会为你打开。

| 课程                   | 说明                                                         |
| :--------------------- | :----------------------------------------------------------- |
| 人工智能与机器学习     | 深度学习、强化学习、LLM 与多模态。入门推荐 [吴恩达的 Machine Learning Specialization](https://www.coursera.org/specializations/machine-learning-introduction)，再深入 [CS231n](https://cs231n.stanford.edu/) 与 [CS224n](https://web.stanford.edu/class/cs224n/)。 |
| 软件工程与应用开发     | 前后端、全栈、架构与云原生开发。入门可从 [The Odin Project](https://www.theodinproject.com/) 或 [Full Stack Open](https://fullstackopen.com/en/) 开始，边写边部署。 |
| 计算机系统             | 体系结构、编译、并行与内核开发。推荐 [UCB CS61C](https://cs61c.org/) 与被誉为神书的 [CSAPP](https://csapp.cs.cmu.edu/)，并行方向看 [CMU 15-418](https://www.cs.cmu.edu/~15418/)。 |
| 分布式系统与云计算     | 一致性、共识、算法与大规模系统设计。首选 [MIT 6.5840](https://pdos.csail.mit.edu/6.824/)，5 个 Lab 带你实现基于 Raft 的 KV 存储。 |
| 计算机网络与信息安全   | 网络协议、密码学、Web 与系统安全。理论基础看 [UCB CS161](https://cs161.org/)，动手实验跟 [SEED Labs](https://seedsecuritylabs.org/)。 |
| 计算机视觉             | 图像处理、检测分割、3D 视觉与视频。入门神课 Stanford [CS231n](https://cs231n.stanford.edu/)，作业从零实现反向传播与卷积。 |
| 自然语言处理           | 语言模型、序列建模、信息抽取与检索。推荐 Stanford [CS224n](https://web.stanford.edu/class/cs224n/)，进阶读 Hugging Face 的 [NLP Course](https://huggingface.co/learn/nlp-course)。 |
| 机器人与自主系统       | 运动规划、控制、SLAM 与自动驾驶。入门看宾大的 [Robotics Specialization](https://www.coursera.org/specializations/robotics)，SLAM 读高翔的[《视觉 SLAM 十四讲》](https://github.com/Gaoyao/SLAM-BOOK)。 |
| 计算机图形学与游戏开发 | 渲染、光线追踪、着色器与游戏引擎。入门首选 [UCB CS184](https://cs184.eecs.berkeley.edu/)，进阶做一遍 [《Ray Tracing in One Weekend》](https://raytracing.github.io/)。 |
| 数据科学与大数据       | 数据分析、挖掘、数据工程与流处理。从 [Kaggle Learn](https://www.kaggle.com/learn) 快速上手并打一场比赛，数据工程看 [data-engineering-zoomcamp](https://github.com/DataTalksClub/data-engineering-zoomcamp)。 |

## 职业发展与就业

> _不患无位，患所以立。_

技术和岗位不是一回事：会写代码的人多，能讲清自己做过什么、为什么这么做的人少。这一节的核心是把学习成果转化为证据，包括能跑的项目、可读的仓库、清楚的文档，以及面试中讲明技术选择的能力。尽早开始积累，实习和求职的准备往往需要几个学期，而不是临时抱佛脚。

| 课程               | 说明                                                         |
| :----------------- | :----------------------------------------------------------- |
| 职业方向认知       | 了解各类岗位职责与能力要求。多读招聘网站的 JD，参考 [levels.fyi](https://www.levels.fyi/) 看清各岗位的职级要求。 |
| 项目经验与作品集   | 项目选题、部署演示、GitHub 与技术博客。一个能点开、能运行、讲得清楚的项目，比“熟悉 XX 技术”更有说服力。 |
| 实习与求职准备     | 简历、算法与工程面试、系统设计面试。算法刷 [LeetCode](https://leetcode.cn/)，系统设计必读 [System Design Primer](https://github.com/donnemartin/system-design-primer)。 |
| 科研与学术发展     | 文献阅读、实验复现、论文写作与申请。入门读 [《How to Read a Paper》](https://web.stanford.edu/class/ee384m/Handouts/HowtoReadPaper.pdf)，文献管理用 Zotero，排版用 LaTeX。 |
| 技术沟通与团队协作 | 文档编写、代码审查、项目管理与表达。推荐 Google 的 [Technical Writing Courses](https://developers.google.com/tech-writing) 与 [工程实践文档](https://github.com/google/eng-practices)。 |
| 持续学习与职业成长 | 跟踪技术趋势、评估新技术、长期规划。读官方文档而非二手教程，关注 [Hacker News](https://news.ycombinator.com/) 保持输入。 |



## 定制路线

> _授人以鱼不如授人以渔_

以上的课程规划难免带有强烈的个人偏好，不一定适合所有人，更多是起到抛砖引玉的作用。如果你想挑选自己感兴趣的方向和内容加以学习，可以参考我在下面列出来的资源。

- [MIT OpenCourseWare](https://ocw.mit.edu/): 麻省理工学院的课程资源开放共享项目，收录了数以千计的各科课程资源，其中计算机类的课号是 6.xxx。
- [MIT CS Course List](http://student.mit.edu/catalog/m6a.html): 麻省理工学院的 CS 课程列表。
- [UC Berkeley EECS Course Map](https://hkn.eecs.berkeley.edu/courseguides): UC Berkeley 的 EECS 培养方案，以课程地图的方式将各门课程的类别和先修关系一目了然地呈现，其中绝大多数课程本书中均有收录。
- [UC Berkeley CS Course List](https://www2.eecs.berkeley.edu/Courses/CS/): UC Berkeley 的 CS 课程列表。
- [Stanford CS Course List](https://blog.csdn.net/qq_41220023/article/details/81976967): 斯坦福的 CS 课程列表。