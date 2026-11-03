<figure markdown>
  ![Image title](./images/title_light.png#only-light){ width="100%" }
  ![Image title](./images/title_dark.png#only-dark){ width="100%" }
</figure>
# Foreword

This book is an open-source, free guide to a computer science curriculum for the AI era. It is a gift to the juniors who come after me, and my small contribution to the open-source community.

If this guide helps you even a little, that will be encouragement and comfort enough for me.

The book currently contains the following parts (if you have better ideas, or would like to join the contributors, feel free to reach me at [zhangchaowen@stu.scu.edu.cn](mailto:zhangchaowen@stu.scu.edu.cn), or open an [Issue](https://github.com/George-102/AICS_Learning_Guide/issues)):

- **How to Use This Guide**: the book covers a great many resources, so I have written usage guides for readers with different amounts of free time and different learning goals.
- **AICS Learning Plan**: a learning plan for the AI era of computer science, for reference only.

## Where the Journey Began

When I entered university I was a complete beginner in computing. Apart from playing PC games, I could not even install legitimate software. Still, I began my computer science journey with curiosity and enthusiasm. Every day I went to class on time, listened attentively to the lectures, took careful notes, and completed the assignments. Yet I gradually realized that every teacher taught differently, at a different pace, with different emphases and different levels of enthusiasm. Some merely read out an outdated slide deck; some did little more than call on students to answer questions already printed on the slides. Very few were genuinely committed to teaching and to making students think critically. Day after day of this dull routine wore my enthusiasm down... I lost my bearings, and for a while I wondered whether computer science was simply not for me, because everything I had imagined about geeks as a child had been shattered by my first year. I kept asking myself: if AI can do so many things, what do I actually need to learn? Do I still need to learn Java and Python? Do I still need data structures and computer networks? I assumed my university years would pass quietly like this: classes, studying, entertainment. Then, within a couple of months, DeepSeek-V3 arrived on the scene, and everyone around me was raving about this brand-new model.

As a beginner, I thought it was no big deal — just one more tool to help me write code. I went on grinding through the four core courses in their conventional order, just as before, until near the start of my second year, when my data structures teacher happened to share a post in the group chat: the text of Andrew Ng's talk at a Buildathon. The moment I saw it I was hooked. I read the whole thing in one sitting, and still unsatisfied, went to YouTube to watch the original video.

The talk was about AI-assisted programming, rapid prototyping, and the skills an AI engineer needs. For the first time I saw clearly where this industry — and every industry — is heading: **understand AI and master AI**.

From Andrew Ng's talk I drew several key ideas:

- **"Move fast and take responsibility."** AI-assisted programming brings a tenfold speed-up to solo prototype development. When the cost of a prototype falls dramatically, rapid and repeated trial and error becomes a viable strategy, and the real value lies in discovering, through that trial and error, the projects worth developing seriously.

- **Code is depreciating, and developers must become system designers and AI conductors.** Programming tools have already gone through several generations: from GitHub Copilot to IDE integration to highly agentic coding assistants. Tools iterate fast enough to create real gaps in productivity, and falling half a generation behind can significantly limit your output. The value of code itself is declining. AI can generate code and migrate database schemas automatically, which makes architectural decisions far more reversible. Developers must shift from writing code to designing systems and conducting AI, focusing on core architecture and building composite systems.

- **"You don't need to learn programming in the AI era" is the worst career advice ever given.** Andrew Ng strongly rejects this idea, pointing out that every advance in programming tools in history has enabled more people to program. His team's CFO, legal counsel and receptionist all learned to program and improved their productivity as a result. The core skill of the future is "telling the computer precisely what to do," which requires understanding computer languages and programming logic. Non-technical people can acquire basic programming ability quickly with AI assistance and boost their efficiency across domains.

- **AI engineers are scarce, yet university curricula are badly out of date.** The unemployment rate for computer science graduates has risen to 7%, while companies still face a severe shortage of AI engineers. The core contradiction is that university courses fail to cover the key skills in time: AI-assisted programming, LLM API usage, building RAG and agentic workflows, and structured error analysis. The emerging AI engineer needs three capabilities: proficiency with the latest AI coding tools, familiarity with AI building blocks (prompt engineering, evaluation techniques, MCP), and the ability to prototype quickly with basic product intuition.

After that, I began teaching myself along the directions Andrew Ng suggested. I gradually drifted away from university lectures and found many high-quality course resources in the process. With courses like these, you have nothing to worry about: effort, seriousness and time are all it takes. The frustration I had felt in class — having energy but nowhere to put it, putting in endless hours with no return — vanished. This suited me perfectly, and I fell in love with self-directed learning.

If you too are struggling with computer science and share my confusion, take a look at Professor Ng's [Buildathon talk](https://youtu.be/kjg45_5WhqI?si=lcWv2E-pLhF-5StY), because that is where my heart was first set on this path.

## Why This Book

While studying operating systems in the autumn of my second year, I found the lectures dreadfully dull: many examples were ten years old, and the lab guide dated back thirteen years. Talking with friends, I could also feel everyone's worry about the rapid rise of AI and anxiety about future employment. By then I had been self-studying for over a year and had collected a lot of resources, so I shared them with my friends — after all, who would not want to enjoy university life, land a good job, or get into graduate school?

After another year of accumulation, the resources had grown substantial, covering most courses in computer science, intelligence and software engineering programs. I also set up a separate GitHub repository for each course, collecting study materials and my own assignment solutions. Later, while counting credits, I opened my own degree plan and found that it had become a subset of my self-study repository — only two years after I started. Then a bold idea took shape: perhaps I could build a self-study curriculum, recording the pitfalls and paths I had met over three years of self-teaching, combining them with my thinking about the AI era, and offering something small to the CS students who come after me.

## Self-Study or Not?

The greatest benefit of self-study is that you can adjust your pace entirely according to your own progress. You can change your plan at any time and go at your own speed, instead of being constrained by a degree plan and a classroom.

Another benefit is drawing on the best of many sources. The first time I installed a dual-boot system on my laptop I made a mistake and wiped Windows. The only saving grace was that I had no precious data at the time. Later I learned that modern SSDs do not erase data permanently: as long as the new system has not occupied that part of the disk, the data may still be recoverable. It was precisely through such mistakes that I kept learning things I would never have encountered otherwise.

A third benefit is freedom over your time. University life is already relatively free, and self-study frees you further to arrange your own schedule and plan. With sensible time management, you can study independently and still get good grades.

Are there downsides? Of course — every rose has its thorn.

The first is that it is hard to ask for help. The problem you run into may be one nobody else has hit, or nobody cares about. Still, asking well on Google, StackOverflow and AI platforms can solve 90% of your problems. The second is that many excellent courses and resources are in English, but that is no longer a serious obstacle, since translation tools and browser extensions now handle it almost perfectly. The third, and by far the hardest, is self-discipline. Having no deadlines is a truly frightening situation. As the material deepens, the difficulty rises, and finishing an entire course is a punishing grind. You need enough drive to force yourself to sit down, understand thousand-line codebases, and endure hours of debugging. And all of it comes with no credit, no GPA, no teacher, no classmates — only one conviction: you are getting stronger.

## Who This Book Is For

Anyone who is motivated to learn and use computer science well can consult this book. If you already have some foundation and are only interested in one particular field, pick the parts that interest you. And if you, like me back then, know nothing about computing and have just entered university, I hope this book can serve as your walkthrough, so that you spend the least time acquiring the knowledge and skills you need. In a sense, this book is more like a course search engine ordered by my own experience, helping you sample excellent computer science courses without leaving home.

## Special Thanks

Here I would like to sincerely thank, with great respect, all the professors and developers who have open-sourced their course materials for free. Those courses and resources embody decades of accumulated teaching experience and dedication, and their authors chose selflessly to let everyone enjoy such high-quality CS education. Without them, my university life would not have been so full and joyful. Many professors even replied with long emails of hundreds of words after receiving my thank-you notes, which moved me deeply. They remind me constantly: whatever you do — studying, research, or simply being a decent person — do it with your whole heart.

## Join the Contributors

One person's strength is ultimately limited. I wrote this book late at night in the gaps of a heavy research schedule, so it is bound to have imperfections. Moreover, since my own work is in applied computing, many of the courses emphasize hands-on practice and cover relatively little mathematics, theoretical computer science, or advanced algorithms. If you have rich self-study experience and resources in other fields, you are welcome to open a Pull Request in the project, or contact me by email ([zhangchaowen@stu.scu.edu.cn](mailto:zhangchaowen@stu.scu.edu.cn)).

## Discussion Groups

This book supports comments on its pages. If you want to study a course together with others, you can set up a group chat (QQ or WeChat both work), then leave a comment under the corresponding course page stating your learning goal and how to join. Besides, quite a few readers have already set up groups in Issues, which you can join directly.

## Buy the Author a Cup of Tea

The content of this book is entirely open-source and free. If you find this project helpful, you can star the repository, or buy the author a cup of afternoon tea.

<figure markdown>
  ![Image title](./images/sponsor.jpg){ width="500" }
</figure>