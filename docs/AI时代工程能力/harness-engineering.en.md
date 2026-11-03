# Harness Engineering

## Descriptions

- Offered by: An open source community course by walkinglabs ([course website](https://walkinglabs.github.io/learn-harness-engineering/)), not a for-credit university course, released as a series of short lessons
- Prerequisites: A real code repository, familiarity with Git and the command line, and having used at least one coding agent (such as Claude Code or Codex)
- Programming Languages: None in particular. The course focuses on instruction files, configuration, and verification commands inside a repository, with possibly a little Shell or Python for verification hooks
- Difficulty: 🌟🌟
- Class Hour: About 12 lessons, roughly 8 hours of reading, plus at least 15 hours of practice in your own project

<!-- 
        Introduce the course in a paragraph or two, including but not limited to:
        (1) The technical knowledge covered in lectures
        (2) Its differences and features compared to similar courses
        (3) Your personal experiences and feelings after studying this course
        (4) Caveats about studying this course on your own (pitfalls, difficulty warnings, etc.)
        (5) ... ...
-->

This course discusses a very plain question: a capable model does not mean it works reliably in your repository. The word "harness" is used more and more in the AI coding agent community, but most people who say harness actually mean a prompt file. A prompt file is not a harness.

This lesson gives harness a precise, actionable definition. Not an abstract concept from an academic paper, but a framework you can use today. A harness consists of five subsystems: instructions, tools, environment, state, and feedback. Each subsystem has a clear responsibility and clear criteria for judging it.

Learn Harness Engineering is a course focused on putting AI coding agents into production engineering practice. Through deliberate environment design, state management, and verification and control mechanisms, it helps you make AI agents such as Codex and Claude Code reliably complete real engineering tasks. By constraining your AI coding assistant with explicit rules and boundaries, it helps you build features, fix bugs, and automate development tasks more reliably.

The first pitfall in self-study is the lack of a real project. Without a repository to work on, the course quickly degenerates into memorizing concepts, so pick a project you maintain that has some complexity and requires running tests as your practice ground. The second pitfall is over-engineering: trying to build a perfect harness from the start leads to ever more configuration files and verification commands nobody maintains, which only adds burden. The course emphasizes "make it reliable first, then make it elegant", and starting from the smallest workable verification loop is more realistic. The third pitfall is treating second-hand interpretations as course conclusions. Harness Engineering is a recently popular concept whose translations and terminology are not yet unified, and many interpretations exaggerate. When you hit a key claim, go back to the original lessons and OpenAI's harness engineering article to verify it.

## Course Resources

- Course Website: <https://walkinglabs.github.io/learn-harness-engineering/>

## Personal Resources

[Official GitHub repository](https://github.com/walkinglabs/learn-harness-engineering/tree/main)