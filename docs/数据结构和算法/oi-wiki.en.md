# OI Wiki

## Descriptions

- Offered by: OI Wiki an open source knowledge base ([course website](https://en.oi-wiki.org/)) maintained by contributors under the CC BY-SA 4.0 license with English content updated continuously
- Prerequisites: Basic C/C++ syntax and standard library, familiarity with the basic operations on arrays and strings, and the ability to read complexity notation
- Programming Languages: Mostly C++, with some entries also available in Python and Java, in a contest-oriented coding style
- Difficulty: 🌟🌟🌟🌟
- Class Hour: About 80 hours for a systematic read of the basic and advanced parts, or more than 150 hours to go deep by topic with targeted practice

OI Wiki is a knowledge base for competitive programming (OI). Instead of being taught over a semester, it organizes topics as encyclopedic entries. The content falls into three blocks. The basics cover language fundamentals, complexity analysis, enumeration, simulation, recursion, greedy algorithms, binary search, searching, introductory dynamic programming, and string basics. The advanced part covers dynamic programming variants such as bitmask DP, tree DP, and slope optimization, plus data structures including union-find, Fenwick trees, segment trees, and balanced trees, along with graph modeling, network flow, and a wide range of string algorithms. The mathematics and contest-technique block covers number theory, combinatorics, linear algebra, polynomials, and game theory, as well as how these data structures and algorithms combine in real problems.

Its defining trait is completeness and depth. Topics almost absent from textbooks yet repeatedly tested in contests, such as persistent segment trees, link-cut trees, dynamic trees, and the Min_25 sieve, each have their own entry with derivations, template code, and linked examples, spanning everything from beginner level to provincial team and beyond. An entry typically states the definition and the naive idea first, then derives the optimization, and finally gives complexity and a code template, with references in the footer so you can follow the trail to original papers and blogs. Compared with introductory books such as *Hello Algo*, it does not aim for a smooth learning curve; compared with scattered contest blogs, it keeps terminology consistent and structure clear, so a tool does not change names and implementations from page to page, which matters a lot for building a coherent framework.

The reading experience is closer to a reference manual than a textbook. Individual entries are dense with formulas and code and lack narrative continuity or designed exercises, so a first pass is hard to read straight through. It is better used with specific questions in hand. The upside is that you jump straight to what you need rather than following a fixed chapter order; the downside is fragmentation, where you have read the definition of a balanced tree but cannot write a rotation, or know the network flow template but cannot tell which problems should be modeled that way. Use it as a dictionary and a tool for deep dives into individual topics, and pair it with a tutorial or course that provides a teaching order and the big picture.

The first pitfall is diving into advanced entries without filtering prerequisites. Segment trees and balanced trees assume you are comfortable with recursion, tree structures, and pointer manipulation; jumping straight into the templates only lets you memorize code without understanding it, so first work through the basics plus recursion, binary search, and union-find. The second pitfall is treating templates as answers. The OI Wiki templates are usually not the optimal implementation, and copying them blindly skips the reasoning and leaves you unable to transfer the idea to variants, so re-implement every template yourself and rename the variables to understand the details. The third pitfall is ignoring the mathematics entries. Number theory, combinatorics, and matrix exponentiation are often the dividing line in contests and the driest to read, so look them up when a problem type demands them instead of reading them front to back, which usually ends in abandoning them.

## Course Resources

- Course Website: <https://en.oi-wiki.org/>

## Personal Resources

[Official GitHub repository](https://github.com/OI-wiki/OI-wiki)