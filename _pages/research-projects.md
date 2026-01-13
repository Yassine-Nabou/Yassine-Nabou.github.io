---
title: "Research Projects"
permalink: /research-projects/
author_profile: true
---

## Optimized first-order methods for convex optimization  
With François Glineur and Julien Hendrickx, we derived several numerical methods for designing optimized first-order algorithms in unconstrained convex optimization settings. Our methods are based on the Performance Estimation Problem (PEP) framework, which casts the worst-case analysis of optimization algorithms as an optimization problem itself. We applied our methods to numerically tune the step sizes of several fixed-step first-order algorithms—namely coordinate descent, inexact gradient descent, and cyclic gradient descent—in the context of linear convergence. These methods provide accelerated convergence rates compared to those of classical algorithms.

I presented these results at Europt 2024, ISMP 2024, and Algopt24.  
[Paper](https://arxiv.org/abs/2507.20773) · [Code](https://github.com/yassinekamri/Numerical-Design-of-First-Order-Optimized-Algorithms) · [Slides](https://drive.google.com/file/d/1SxXV-4ts8Di0s3V9ALdd2gp_NxLv2Loz/view?usp=sharing)

---

## Worst-case analysis of block coordinate descent algorithms  
With François Glineur and Julien Hendrickx, we extended the Performance Estimation Problem (PEP) framework for the worst-case analysis of block coordinate descent algorithms.  

First, we proposed a convex PEP framework for these algorithms over smooth convex functions, which led to the publication of a conference paper at ECC23. This framework enables sharp performance guarantees in that setting.  
[Paper](https://ieeexplore.ieee.org/abstract/document/10178198)  · [Slides](https://drive.google.com/file/d/1Ch0rS53Mg2s6EtOxztGbvUAjxgSYb3ZQ/view?usp=sharing)

We then extended our work by deriving a convex PEP framework for the worst-case analysis of block coordinate descent algorithms over the class of coordinate-wise smooth convex functions, which is the standard class used to analyze such algorithms. This framework generalizes the analysis and provides insights into algorithmic behavior. I presented these results at Europt23 and SIAMOP23.  
[Paper](https://arxiv.org/abs/2507.16675) · [Code](https://github.com/yassinekamri/PEPs-Block-Coordinate-Descent-Algorithms) · [Slides](https://drive.google.com/file/d/1Cd_IUJK2Zu0karDKNZFG7nXlfw-Jl6nq/view?usp=sharing)

---

## Faster optimization methods for day-ahead electricity markets  
With Sofiane Tanji, Mehdi Madani, and François Glineur, we conducted extensive benchmarking experiments for convex hull price computation on a large panel of first-order methods. We then proposed methods combined with heuristics to efficiently solve convex hull pricing. These approaches improve scalability for large-scale electricity market instances.  
[Paper](https://arxiv.org/abs/2504.01474) · [Code](https://github.com/SofianeTanji/ConvexHullPricing.jl)

---

## Constrained Policy Optimization for Load Balancing  
With P. T. A. Quang, N. Huin, and J. Leguay, during my master's thesis I applied deep reinforcement learning to the task of load balancing in telecommunication networks, which led to a conference paper at the 17th International Conference on the Design of Reliable Communication Networks (DRCN). This work demonstrates that constrained policy optimization can improve network reliability under traffic uncertainty.  
[Paper](https://ieeexplore.ieee.org/abstract/document/9477375)

