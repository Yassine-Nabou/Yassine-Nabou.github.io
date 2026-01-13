---
title: "Dual first-order methods for efficient computation of convex hull prices"
collection: publications
category: manuscripts
permalink: /publication/cvx_hull_pricing
excerpt: ''
date: 2025-04-02
venue: 'ArXiv'
paperurl: 'https://arxiv.org/abs/2504.01474'
citation: 'S. Tanji, Y. Kamri, F. Glineur, and M. Madani. Dual First-Order Methods for Efficient Computation of Convex Hull Prices. arXiv, 2025.'
---

Convex Hull (CH) pricing, used in US electricity markets and raising interest in Europe, is a pricing rule designed to handle markets with non-convexities such as startup costs and minimum up and down times. In such markets, the market operator makes side payments to generators to cover lost opportunity costs, and CH prices minimize the total "lost opportunity costs", which include both actual losses and missed profit opportunities. These prices can also be obtained by solving a (partial) Lagrangian dual of the original mixed-integer program, where power balance constraints are dualized. Computing CH prices then amounts to minimizing a sum of nonsmooth convex objective functions, where each term depends only on a single generator. The subgradient of each of those terms can be obtained independently by solving smaller mixed-integer programs. In this work, we benchmark a large panel of first-order methods to solve the above dual CH pricing problem. We test several dual methods, most of which not previously considered for CH pricing, namely a proximal variant of the bundle level method, subgradient methods with three different stepsize strategies, two recent parameter-free methods and an accelerated gradient method combined with smoothing. We compare those methods on two representative sets of real-world large-scale instances and complement the comparison with a (Dantzig-Wolfe) primal column generation method shown to be efficient at computing CH prices, for reference. Our numerical experiments show that the bundle proximal level method and two variants of the subgradient method perform the best among all dual methods and compare favorably with the Dantzig-Wolfe primal method.