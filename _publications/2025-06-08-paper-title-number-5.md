---
title: "Constrained Policy Optimization for Load Balancing"
collection: publications
category: conferences
permalink: /publication/paper_master_thesis
excerpt: ''
date: 2021-04-19
venue: '2021 17th International Conference on the Design of Reliable Communication Networks (DRCN)'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/9477375'
citation: 'Y. Kamri, P. T. A. Quang, N. Huin and J. Leguay, "Constrained Policy Optimization for Load Balancing," 2021 17th International Conference on the Design of Reliable Communication Networks (DRCN), Milano, Italy, 2021, pp. 1-6'
---

To improve the bandwidth utilization in IP networks, a centralized controller splits flow aggregates over multiple paths and decides load balancing weights. Ideally, load balancing policies should anticipate the impact of their decisions on the Quality of Service (QoS). However, the embedding of accurate performance models into load balancing optimization algorithms is a challenge. In this context, we propose a Deep Reinforcement Learning (DRL) based solution that is able to learn the relationship between traffic and QoS, while providing safety to maximize throughput and avoid violating link capacity constraints. Our safe solution for QoS-aware load balancing integrates DRL algorithms with the Reward Constrained Policy Optimization algorithm. In a scenario where link delays follow the M/M/1 queuing model, we demonstrate, using a non-linear integer program, that our solution can reach a close to optimal end-to-end delay. We also show that our solution automatically learns reward parameters to meet capacity constraints.
