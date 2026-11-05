# Git

## Descriptions

- Offered by: The Learn Git Branching open source interactive tutorial ([course website](https://learngitbranching.js.org/?locale=en_US)), published as a visual sandbox that runs inside the browser
- Prerequisites: No experience with Git or a graphical client is required; you only need to be able to use a command line (knowing basics such as `cd` and `ls`) and to have a rough idea that "version control" exists to keep a history of versions
- Difficulty: 🌟
- Class Hour: About 8 hours for the main and remote repository parts, or 15 hours to read everything and finish all the challenge levels

It turns Git's branch operations into playable levels. The tutorial is organized around several core level groups: the basics cover `commit`, `branch`, `merge`, and `rebase`; the advanced part covers `checkout`, `reset`, `revert`, `cherry-pick`, and interactive `rebase` for moving between commits; then come groups on "moving commits around", "miscellaneous", and "advanced topics", and finally the remote repository part covering `clone`, `fetch`, `pull`, `push`, tracking branches, and remote branches. Each level has one clear goal, with a visual repository graph on the right; once you type a command, the commit nodes and branch pointers move immediately, and reaching the goal completes the level. Progress is stored locally in the browser.

Its biggest strength is turning the abstract branch model directly into an image. The most confusing part of Git is the mental model where "commits are nodes, branches are pointers, and HEAD is the current position", and no amount of writing that in a handout beats actually using `git rebase` to attach a detached commit onto another branch and watching the nodes rearrange in the graph. Second, every level demonstrates first and then asks you to practice, with a short explanation and command hints on the left and `undo` and `reset` always available on the right, so failure costs nothing; you can experiment boldly in a way that is impossible in a real repository. Compared with systematic texts such as *Pro Git*, it does not walk through principles and configuration item by item; compared with scattered Git cheatsheets, it offers a progressive order and immediate feedback.

## Course Resources

- Course Website: <https://learngitbranching.js.org/?locale=en_US>
- Textbooks: Pair it with *Pro Git* ([free online](https://git-scm.com/book/en/v2)) to fill in principles and configuration

## Personal Resources

[Official GitHub repository](https://github.com/pcottle/learnGitBranching)