# TOOL-101: Learning Git Branching

## Descriptions

- Offered by: Learn Git Branching, an open source interactive tutorial ([course website](https://learngitbranching.js.org/?locale=zh_CN)), released as an in-browser visual sandbox
- Prerequisites: No Git or GUI client experience needed; basic command line skills (`cd`, `ls`, and so on) and a rough idea that version control keeps history of changes are enough
- Programming Languages: None; learners clear levels by typing Git commands
- Difficulty: 🌟
- Class Hour: About 8 hours for the main and remote sections, or around 15 hours to finish everything including the challenge levels

It turns Git's branching model into playable levels. The tutorial is organized around several level groups: the basics cover `commit`, `branch`, `merge`, and `rebase`; the advanced group covers moving around commits with `checkout`, `reset`, `revert`, `cherry-pick`, and interactive `rebase`; then come groups such as "moving commits around", "miscellaneous", and "advanced topics"; the remote section closes with `clone`, `fetch`, `pull`, `push`, tracking branches, and remote-tracking branches. Each level has a single clear goal, the repository graph sits on the right, and commit nodes and branch pointers move immediately as you type a command. Clearing the goal completes the level, and progress is saved locally in the browser.

Its biggest advantage is turning an abstract branching model into an image. The confusing part of Git is the mental model of commits as nodes, branches as pointers, and HEAD as your current position, and no handout repeated ten times beats actually running `git rebase` to attach a detached commit to another branch and watching the nodes rearrange in the graph. Second, every level demonstrates first and then lets you practice: there is a short explanation and command hints on the left, and the right side always supports `undo` and `reset`, so failure costs nothing and you can experiment freely, which is impossible in a real repository. Compared with systematic books such as *Pro Git*, it does not walk through principles and configuration item by item; compared with scattered Git cheat sheets, it offers a gradual order and immediate feedback.

## Course Resources

- Course Website: <https://learngitbranching.js.org/?locale=zh_CN>
- Textbooks: Pair it with *Pro Git* ([free Chinese edition online](https://git-scm.com/book/zh/v2)) for principles and configuration

## Personal Resources

[Official GitHub repository](https://github.com/pcottle/learnGitBranching)