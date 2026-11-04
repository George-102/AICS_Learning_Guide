# TOOL-105: CMake

## Descriptions

- Offered by: The official CMake tutorial and training material from the IPADS group at Shanghai Jiao Tong University ([CMake website](https://cmake.org/))
- Prerequisites: First learn GNU Make and Makefile basics, including targets, prerequisites, and incremental builds
- Programming Languages: Mostly C/C++, with build scripts written in CMakeLists.txt
- Difficulty: 🌟🌟🌟🌟
- Class Hour: About 10 hours for the official tutorial, or 20 or more hours to organize builds independently in a cross-platform project

CMake is a layer of abstraction above GNU Make: instead of compiling directly, it generates build files. You write CMakeLists.txt to describe which targets exist, which libraries each depends on, and which compile options are needed, and CMake turns that into a Makefile, a Ninja file, or a Visual Studio project for each platform. One configuration then works on Linux, macOS, and Windows, with no per-platform script to maintain, which is precisely why it became the de facto standard of the C/C++ ecosystem.

The cost is that higher abstraction is harder to reason about. A Makefile lets you see line by line what runs, while CMakeLists.txt requires a mental picture of "the configure stage generates the build stage"; without it, error messages make no sense. Modern CMake also introduced target-based style, propagating usage requirements through `target_link_libraries` and `target_include_directories`. That is much cleaner than the old global-variable approach but also makes it easier to get lost among half-old, half-new tutorials.

IDEs deserve a mention. Visual Studio and CLion can generate CMakeLists.txt automatically, and in daily work you may never write one by hand; but the moment you add third-party libraries, define install rules, or handle conditional compilation, generated configs usually fall short, and whether you can fix them becomes the dividing line. Even with tooling doing the work, understanding the basics remains necessary.

The first pitfall is skipping Make. CMake is fundamentally a Makefile generator, so without understanding targets and prerequisites you tend to write CMakeLists.txt as a flat list of commands and lose every benefit of incremental and cross-platform builds. The second pitfall is mixing old and new styles. Many online tutorials still use global commands such as `include_directories` and `link_directories`, which spread dependencies across the whole project and produce mysterious header conflicts; stick to target-based style. The third pitfall is refusing to get hands-on. Build system knowledge only grows from building a multi-directory, multi-target project from scratch and gradually adding third-party dependencies; reading the official tutorial alone rarely sticks.

## Course Resources

- Course Website: <https://cmake.org/>
- Recordings: The IPADS group at Shanghai Jiao Tong University provides a roughly one-hour video tutorial
- Textbooks: The official CMake tutorial as the main line, with the official docs for specific questions
- Assignments: No standardized assignments; build a multi-target project with a static library, executables, and unit tests from scratch

## Personal Resources

A reasonable practice path: start with a single-executable project, extract a static library, add a third-party dependency, configure install and export rules, and finally make it build on both Linux and Windows. Each step exposes gaps in your understanding of how targets propagate, and one pass through them means other people's project configs stop looking like ciphertext.