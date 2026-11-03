# RL-101: Easy RL

## Descriptions

- Offered by: The Datawhale open source community tutorial *Easy RL: A Tutorial on Reinforcement Learning* (commonly known as the "Mushroom Book", [course website](https://datawhalechina.github.io/easy-rl/#/)), written by Wang Qi, Yang Yiyuan, and Jiang Ji, with a print edition published by Posts and Telecom Press
- Prerequisites: Comfortable with Python, basic probability (random variables, expectation, conditional probability), linear algebra and calculus, and common deep learning background (neural networks, backpropagation, gradient descent)
- Programming Languages: Python, with code mainly based on PyTorch and Gym
- Difficulty: 🌟🌟🌟
- Class Hour: About 60 hours to read through, or more than 100 hours including running the algorithms and working through the exercises

The course has two major parts. Part one (chapters 1 to 3) builds the foundation: how reinforcement learning differs from other machine learning paradigms, then Markov decision processes (MP, MRP, and MDP in increasing layers), and tabular methods (Q tables, Sarsa, Q-learning, policy evaluation and improvement). Part two (chapters 4 to 13) moves into deep reinforcement learning, covering model-free prediction and control, deep learning basics, DQN and its variants, DQN for continuous actions, policy gradient, Actor-Critic, DDPG, PPO, and practical problems such as sparse rewards and imitation learning. The chapters of part two are relatively independent and can be read selectively, which gives readers with different goals room to choose.

Its main strengths are being Chinese-language, systematic, and exercise-backed. The book started as an organized expansion of Hung-yi Lee's open course on deep reinforcement learning along with lecture notes from Bolei Zhou, David Silver, and others, filling in derivations that jump abruptly in the videos. Every chapter ends with exercises and solutions, so it does not read like a scattered survey. Compared with Sutton's *Reinforcement Learning*, which is theory-first and extremely dense, it leans toward engineering implementation and intuition building. Compared with open source RL code repositories, it does not skip steps and explains why each algorithm is designed the way it is. The community consensus is that the book is readable, and I think that comes from keeping the derivations while pairing them with many figures and plain Chinese explanations.

The experience has a clear steep section. The first three chapters are easy going, but once DQN arrives, target networks, experience replay, temporal difference, and importance sampling all come at once, and anyone with a shaky deep learning foundation tends to fall behind there. Before starting part two, review neural network training and gradient descent, and think through motivation questions such as why a target network is needed; that is far more effective than memorizing formulas.

The first pitfall is reading without running. Many details of reinforcement learning only surface when the code runs: reward scaling, exploration decay, sample efficiency. Reading alone creates the feeling of understanding, and only a training run that refuses to converge shows where the problem really is. Run at least one environment each for Q-learning, DQN, and PPO. The second pitfall is skipping part one to jump straight into deep reinforcement learning. MDPs, Bellman equations, and temporal difference are the shared language of the field, and a weak grasp there causes repeated stalls later. The third pitfall is being intimidated by the notation. The derivations do require patience, but most steps are basic operations on expectations and gradients; when stuck, revisit the first two chapters or compare with Hung-yi Lee's video lectures, where a single sentence often clears it up. One final warning: the book was written a few years ago, so some library versions and code interfaces have changed, and you should follow the most recent branch of the official repository when running the code.

## Course Resources

- Course Website: <https://datawhalechina.github.io/easy-rl/#/>
- Recordings: Pair it with Hung-yi Lee's open course on deep reinforcement learning; the site itself is mainly text and figures
- Textbooks: *Easy RL: A Tutorial on Reinforcement Learning* (Posts and Telecom Press); the electronic version can be read online for free
- Assignments: Each chapter includes exercises with solutions, complemented by the algorithm implementations and experiment code in the official repository

## Personal Resources

[Official GitHub repository](https://github.com/datawhalechina/easy-rl)