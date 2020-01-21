---
title: 'POMDP'
date: 2020-01-22
permalink: /posts/2012/08/blog-post-1/
tags:
  - pomdp theory
---

POMDP can be described as a tuple $ <\mathcal{S},\mathcal{A}, \mathcal{T}, \mathcal{R}, \Omega> $ where:
- $\mathcal{S, A, T}$ describe a Markov decision process
- $\Omega$ is a finite set of observations the agent can experience of its worlds
-  $\mathcal{O}: \mathcal{S} \times \mathcal{A} \rightarrow \Pi(\Omega)$ is the observation function, which gives, for each action and resulting state, a probability of making observation $o$ given that the agent took action $a$ and landed in state $s'$
A POMDP is an MDP in which the agent is unable to observe the current state. Instead, it makes an observation based on the action and the resulting state. The agent's goal is still the same as in the MDP case.  

What exactly is a belief state? One possible choice might be the most probable state of the world, given the past experience. However, it is not sufficient in general. In order to act effectively, an agent must take into account its own degree of uncertainty. If it is lost or confused, it might be appropriate for it to take sensing actions such as asking for directions, reading a map, or searching for a landmark.
  
The good choice for belief states will be probability distributions over states of the world. These distributions encode the agent's subjective probability about the satte of the world and provide a basis for act under uncertainty. Furthermore, they comprise a _suffificent statistic_ for the past history and initial belief state of the agent: given the agent's current belief state (properly computed), no additional data about its past actions or observations would supply any further information about the current state of the world. This means that the process over belief states is Markov, and that no additional data about the past would help to increase the agent's expected reward.
  
Computing belief states:
A belief state $b$ is a probability distribution over $\mathcal{S}$. We let $b(s)$ denote the probability assigned to world state $s$ by belief state $b$. The state estimator must compute a new belief state $b'$ given an old belief state $b$, an action $a$, and an observation $o$. The new degree of belief state in some state $s'$, $b'(s')$ can be obtained as follows:

$$b'(s') = P(s'|o,a,b) = $$
