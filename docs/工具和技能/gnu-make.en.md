# TOOL-104: GNU Make

## Descriptions

- Offered by: The GNU manual and community tutorials ([GNU Make manual](https://www.gnu.org/software/make/manual/))
- Prerequisites: Able to compile a single source file with GCC (`gcc hello.c -o hello`) and a rough grasp of preprocessing, compilation, assembly, and linking
- Programming Languages: Mostly C/C++, with build scripts written in Makefile syntax
- Difficulty: 🌟🌟
- Class Hour: About 6 hours for the syntax and dependency rules, or 10 or more hours to read and rework a large open source Makefile

Start from a concrete problem. For hello world you edit `hello.c` and one `gcc` command produces the executable. Once a project grows to thousands of source files across dozens of subdirectories, though, you have to compile and link them together somehow; and if a full build takes half an hour, should a one-character change cost another half hour?

GNU Make answers exactly that. A Makefile describes the whole build and declares which source and header files each target depends on, so only the parts affected by your change get rebuilt. This incremental build is the performance foundation of every large C/C++ project, and once you understand it you also understand why touching one header file triggers a mass rebuild: the dependency graph propagates the impact.

It is easy to learn and harder to use well. The syntax is small, and variables, rules, targets, and prerequisites cover most needs; the craft is in writing dependencies that are complete without being redundant, organizing multi-directory layouts, and using pattern rules and automatic variables to cut repetition. There is no single right answer, and the best approach is to read the Makefiles of good open source projects, imitate them, and settle on your own template.

The first pitfall is skipping dependencies to memorize syntax. Almost all of a Makefile's value lives in its dependency declarations, so learning only "run these commands" demotes an incremental build tool to a command alias. The second pitfall is tolerating changes that do not take effect. That usually means a missing dependency or a timestamp problem, and reaching for `make clean` hides it; trace the dependency chain and fix the hole instead, or a slightly larger project will hit the same issue again. The third pitfall is jumping to CMake without a Make foundation. CMake is a higher abstraction, and understanding what CMakeLists.txt ultimately describes requires knowing what it generates, so writing a few real multi-file projects in Make first makes CMake much smoother.

## Course Resources

- Course Website: <https://www.gnu.org/software/make/manual/>
- Textbooks: The official GNU Make manual, ideally paired with a community Chinese tutorial
- Recordings: The manual suffices; no videos needed
- Assignments: No standardized assignments; pick a small open source project and rewrite its build from scratch

## Personal Resources

A good exercise is to start by reading. Take a small or medium C project you know, go through its Makefile, draw the target-dependency graph, then try removing redundant rules and filling in missing dependencies. After a few rounds you gain a complete picture of what really happens during a build.