# Scoop

## 简介

- 来源：Scoop 官方文档与社区实践整理（[Scoop 官网](https://scoop.sh/)）
- 先修要求：熟悉 Windows 下的 PowerShell 基本操作，了解什么是环境变量
- 课程难度：🌟

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

## 资源

- 课程网站：<https://scoop.sh/>

## 资源汇总

进阶方向是 bucket 管理。Scoop 通过 bucket 组织软件来源，除了默认的主库，还有 extras（带图形界面的工具）、versions（历史版本）等常用库，按需添加即可扩大可安装范围。把常装的工具写进一份清单脚本并纳入自己的 dotfiles，新机器上手就再也不用重复劳动了。