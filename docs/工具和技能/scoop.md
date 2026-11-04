# TOOL-107：Scoop

## 课程简介

- 来源：Scoop 官方文档与社区实践整理（[Scoop 官网](https://scoop.sh/)）
- 先修要求：熟悉 Windows 下的 PowerShell 基本操作，了解什么是环境变量
- 编程语言：无，安装与管理各类开发工具，被安装的工具可以是任意语言
- 课程难度：🌟
- 预计学时：安装与常用命令 2 小时，整理出自己的一套日常清单另需数小时

Windows 下搭建开发环境一直是个麻烦事。没有统一标准，每个工具的安装方式都不一样，有的要下载安装包点下一步，有的要解压后手动配环境变量，装十个工具就能耗掉一整天。Scoop 的作用是把这些差异统一掉：它把常见的命令行工具集中管理起来，安装与升级一条命令完成，环境变量也自动处理。

上手极简单，装 Python 与 Node.js 就是两行：

```powershell
scoop install python
scoop install nodejs
```

安装 Scoop 本身需要 PowerShell 5.1 及以上。Windows 10 及以后版本自带，Windows 7 自带的版本太旧，需要先手动升级。这里有个国内用户常踩的细节：不少人设置 Windows 用户时用了中文用户名，用户目录随之变成中文路径，而 Scoop 默认把软件装在用户目录下，部分软件在中文路径下会执行出错。建议用 `-ScoopDir` 参数装到纯英文的自定义目录：

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh -outfile 'install.ps1'
.\install.ps1 -ScoopDir 'C:\Scoop'
```

它最大的好处是把“装软件”变成可重复、可迁移的动作。换一台机器时，把安装清单重新执行一遍就能恢复环境，不用回忆当年每一个安装包的选项。

自学的第一个坑是遇到下载失败就放弃。Scoop 本身只是安装配置的维护者，所有软件都从各自的官方源下载，它并不提供镜像；网络不通时下载会失败，这时需要自己想办法改善网络，而不是去找一个并不存在的“Scoop 镜像源”。第二个坑是装找不到的老版本就以为不支持。社区会把过时弃用的软件从主仓库移到 versions 库，需要时手动加库即可，例如装 Python 2 要执行 `scoop bucket add versions` 再 `scoop install python27`；Java 8 同理，官方已不提供下载链接，可用 ojdkbuild8 替代。第三个坑是不看官方文档。Scoop 的文档对新手很友好，快速入门一页就能覆盖大部分场景，比自己摸索要快得多。

## 课程资源

- 课程网站：<https://scoop.sh/>
- 课程教材：Scoop 官方文档中的快速入门章节
- 课程视频：无，文档足以覆盖
- 课程作业：无标准化作业，建议把自己的常用工具整理成一份可重复执行的安装脚本

## 资源汇总

进阶方向是 bucket 管理。Scoop 通过 bucket 组织软件来源，除了默认的主库，还有 extras（带图形界面的工具）、versions（历史版本）等常用库，按需添加即可扩大可安装范围。把常装的工具写进一份清单脚本并纳入自己的 dotfiles，新机器上手就再也不用重复劳动了。