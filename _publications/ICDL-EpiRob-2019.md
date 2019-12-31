---
title: "Hindsight Experience Replay With Experience Ranking"
collection: publications
permalink: /publications/ICDL-EpiRob-2019
venue: "2019 Joint IEEE 9th International Conference on Development and Learning and Epigenetic Robotics (ICDL-EpiRob)"
date: 2019-4-14
citation: '<b>Hai Nguyen</b>, Hung Manh La, Matthew Deans. <i> International Conference on Development and Learning and Epigenetic Robotics.</i> <b>ICDL-EpiRob 2019</b>.'
---
[[PDF]](http://hai-h-nguyen.github.io/files/icdl-epirob.pdf)

## Abstract
Reinforcement Learning (RL) algorithms face difficulties when dealing with robotic tasks in sparse reward settings and as a result, they often require millions of interactions with the environment to learn successfully. A recent algorithm Hindsight Experience Replay (HER) was introduced to tackle this difficulty by adding virtual goals and therefore increase significantly the sample-efficiency by learning in transitions when the robot does not achieve the original goal. However, these additional goals are sampled randomly from each episode batch of transitions, which might have no relationship with the original goal. This might make learning with the original goal slower due to the bad influence of irrelevant virtual goals. In this paper, we address this issue by applying experience ranking (ER) to these additional goals. 
