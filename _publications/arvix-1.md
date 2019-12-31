---
title: "Deep learning with experience ranking convolutional neural network for robot manipulator"
collection: publications
permalink: /publications/arvix-1
venue: "Arxiv 2019"
date: 2019-11-20
citation: '<b>Hai Nguyen</b>, Hung Manh La, Matthew Deans. <i>Arxiv 2019.</i>
---
[[PDF]](https://hai-h-nguyen.github.io/files/arvix-1.pdf)

## Abstract
Supervised learning, more specifically Convolutional Neural Networks (CNN), has surpassed human ability in some visual recognition tasks such as detection of traffic signs, faces and handwritten numbers. On the other hand, even state-of-the-art reinforcement learning (RL) methods have difficulties in environments with sparse and binary rewards. They requires manually shaping reward functions, which might be challenging to come up with. These tasks, however, are trivial to human. One of the reasons that human are better learners in these tasks is that we are embedded with much prior knowledge of the world. These knowledge might be either embedded in our genes or learned from imitation-a type of supervised learning. For that reason, the best way to narrow the gap between machine and human learning ability should be to mimic how we learn so well in various tasks by a combination of RL and supervised learning. Our method, which integrates Deep Deterministic Policy Gradients and Hindsight Experience Replay (RL method specifically dealing with sparse rewards) with an experience ranking CNN, provides a significant speedup over the learning curve on simulated robotics tasks. Experience ranking allows high-reward transitions to be replayed more frequently, and therefore help learn more efficiently. Our proposed approach can also speed up learning in any other tasks that provide additional information for experience ranking.
