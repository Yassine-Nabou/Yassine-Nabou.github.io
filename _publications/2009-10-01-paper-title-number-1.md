---
title: "On the Worst-Case Analysis of Cyclic Block Coordinate Descent type Algorithms"
collection: publications
category: manuscripts
permalink: /publication/coordinate_descent_worstcase
excerpt: ''
date: "2025-07-22"
venue: 'Arxiv'
paperurl: 'https://arxiv.org/abs/2507.16675'
citation: 'Y. Kamri, F. Glineur, J. M. Hendrickx, and I. Necoara. "On the Worst-Case Analysis of Cyclic Block Coordinate Descent Type Algorithms." arXiv, 2025'
---
We study the worst-case behavior of Block Coordinate Descent (BCD) type algorithms for unconstrained minimization of coordinate-wise smooth convex functions. This behavior is indeed not completely understood, and the practical success of these algorithms is not fully explained by current convergence analyses. We extend the recently proposed Performance Estimation Problem (PEP) approach to convex coordinate-wise smooth functions by proposing necessary interpolation conditions. We then exploit this to obtain improved numerical upper bounds on the worst-case convergence rate of three different BCD algorithms, namely Cyclic Coordinate Descent (CCD), Alternating Minimization (AM), and a Cyclic version of the Random Accelerated Coordinate Descent introduced in Fercoq and Richtárik (2015) (CACD)substantially outperforming the best current bounds in some situations. In addition, we show the convergence of the CCD algorithm with more natural assumptions in the context of convex optimization than those typically made in the literature. Our methodology uncovers a number of phenomena, some of which can be formally established. These include a scale-invariance property of the worst case of CCD with respect to the coordinate-wise smoothness constants and a lower bound on the worst-case performance of CCD which is equal to the number of blocks times the worst-case of full gradient descent over the class of smooth convex functions. We also adapt our framework to the analysis of random BCD algorithms, and present numerical results showing that the standard acceleration scheme in Fercoq and Richtárik (2015) appears to be inefficient for deterministic algorithms.
