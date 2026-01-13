---
title: "Numerical Design of Optimized First-Order Algorithms"
collection: publications
category: manuscripts
permalink: /publication/algo_design
excerpt: ''
date: 2025-07-29
venue: 'Arxiv'
paperurl: 'https://arxiv.org/abs/2507.20773'
citation: 'Y. Kamri, J. M. Hendrickx, and F. Glineur. Numerical Design of Optimized First-Order Algorithms. arXiv, 2025.'
---

We derive several numerical methods for designing optimized first-order algorithms in unconstrained convex optimization settings. Our methods are based on the Performance Estimation Problem (PEP) framework, which casts the worst-case analysis of optimization algorithms as an optimization problem itself. We benchmark our methods against existing approaches in the literature on the task of optimizing the step sizes of memoryless gradient descent (which uses only the current gradient for updates) over the class of smooth convex functions. We then apply our methods to numerically tune the step sizes of several memoryless and full (i.e., using all past gradient information for updates) fixed-step first-order algorithms, namely coordinate descent, inexact gradient descent, and cyclic gradient descent, in the context of linear convergence. In all cases, we report accelerated convergence rates compared to those of classical algorithms.