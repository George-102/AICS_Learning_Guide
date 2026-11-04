# TOOL-110: GitHub

## Descriptions

- Offered by: Official GitHub documentation and open source community practice ([GitHub website](https://github.com/))
- Prerequisites: Basic Git operations (commit, branch, remote sync); without them you are limited to clicking around in the browser
- Programming Languages: None; the platform is language agnostic and hosts projects in any language
- Difficulty: 🌟
- Class Hour: About 6 hours for basic usage and collaboration flows, with long-term practice to shape your own open source habits

Functionally, GitHub is an online code hosting platform: push your local Git repository and several people can develop and browse at the same time. Its significance long ago outgrew that definition, and it now feels more like an active open source community where developers worldwide share everything from industrial deep learning frameworks to scripts dozens of lines long. Some publish hardcore technical writing, some write hand-holding tutorials, and many technical books are themselves open sourced in repositories; the guide you are reading is one of them.

Core usage has three layers. The first is hosting and backup, where one `git push` puts your code in the cloud and `clone` brings it back on another machine. The second is collaboration, using branches and pull requests to organize multi-person changes, keeping review in the conversation and tracking issues and discussion with Issues. The third is release and integration, distributing versions through Releases and running tests and builds automatically on every commit with Actions. Only when all three are in use is a repository truly alive.

Its real value is being public and searchable. Whatever problem you hit, someone has likely discussed it in an issue, and whatever tool you need, someone has likely built it as a repository. Learning to search these quickly is far more efficient than writing from scratch, and when you build something useful, publishing it may become someone else's answer.

The first pitfall is treating GitHub as a network drive. A repository is not a dumping ground; without a README, without commit history, and without a clear directory structure, nobody can open or understand it. The second pitfall is committing straight to the main branch. For tiny personal projects it may not matter, but any collaboration calls for branches, pull requests, and review, which is both courtesy and engineering competence. The third pitfall is ignoring open source licenses. The community is not a lawless zone; many projects forbid copying, redistributing, or even reselling their code, so read the LICENSE before using other people's work. That is a legal requirement and a basic responsibility of every community member.

## Course Resources

- Course Website: <https://github.com/>
- Textbooks: The quick start and collaboration sections of the official GitHub documentation
- Recordings: None; the official docs with screenshots are enough
- Assignments: No standardized assignments; run one of your real small projects through the full README, Issue, PR, and Release flow

## Personal Resources

If you have never created a remote repository or cloned someone else's code, start with the official tutorial. To keep discovering interesting projects, follow HelloGitHub, which regularly collects recently popular or intriguing open source projects with a companion WeChat account, solving the "where do I find good stuff" problem.

As for becoming an author whose stars speak for you, the principle is simple: turn the ideas that flash through your development process into code and put them on GitHub generously. Open source works because of the spirit of "all for one, one for all", not because of technique.