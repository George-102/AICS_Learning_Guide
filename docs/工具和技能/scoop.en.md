# Scoop

## Descriptions

- Offered by: Compiled from the official Scoop documentation and community practice ([Scoop website](https://scoop.sh/))
- Prerequisites: Familiarity with basic PowerShell usage on Windows and an idea of what environment variables are
- Difficulty: 🌟

Setting up a development environment on Windows has always been a nuisance. Without a common standard, every tool installs differently: some need a download and a few clicks, some need manual extraction and environment variables, and ten tools can eat an entire day. Scoop removes those differences, managing common command line tools centrally so installation and upgrades take one command and environment variables are handled for you.

Getting started is trivial; installing Python and Node.js takes two lines:

```powershell
scoop install python
scoop install nodejs
```

Scoop itself needs PowerShell 5.1 or later. Windows 10 and newer ship with it, while the version built into Windows 7 is too old and must be upgraded first. One detail that trips up many users in China: people often set a Chinese username when creating their Windows account, which makes the user directory a Chinese path, and since Scoop installs into the user directory by default, some software fails to run there. It is better to install into a custom all-English directory with `-ScoopDir`:

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
irm get.scoop.sh -outfile 'install.ps1'
.\install.ps1 -ScoopDir 'C:\Scoop'
```

Its main benefit is turning software installation into a repeatable, portable action. On a new machine, rerun your installation list to restore the environment instead of recalling what option you chose for every installer years ago.

## Course Resources

- Course Website: <https://scoop.sh/>

## Personal Resources

The next step is bucket management. Scoop organizes software sources as buckets, and beyond the default main bucket there are frequently used ones such as extras (GUI tools) and versions (historical versions); add what you need to widen the catalog. Write the tools you always install into a manifest script and keep it in your dotfiles, and setting up a new machine stops being repetitive work.