---
layout: single
title: "Distributed and Federated Learning"
permalink: /research/distributed-learning/
author_profile: true
---

<style>
.research-page {
  max-width: 1000px;
  margin: 0 auto;
  line-height: 1.75;
}

.research-intro {
  font-size: 1.05em;
  margin-bottom: 1.5em;
}

.research-figure {
  margin: 1.8em 0 2.5em;
  text-align: center;
}

.research-figure img {
  width: 100%;
  height: auto;
  border-radius: 8px;
  border: 1px solid #e5e7eb;
}

.research-figure figcaption {
  margin-top: 0.6em;
  color: #64748b;
  font-size: 0.88em;
}

.research-topic {
  margin: 2.8em 0;
}

.research-topic h2 {
  font-size: 1.4em;
  padding-bottom: 0.45em;
  border-bottom: 1px solid #e5e7eb;
}

.research-highlight {
  margin: 1.2em 0;
  padding: 1em 1.2em;
  border-left: 4px solid #3289b1;
  background: rgba(50, 137, 177, 0.05);
  border-radius: 4px;
}

.research-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.7em;
  margin-top: 1em;
}

.research-links a {
  display: inline-block;
  padding: 0.35em 0.8em;
  border: 1px solid #3289b1;
  border-radius: 4px;
  text-decoration: none;
  font-size: 0.9em;
}

.research-links a:hover {
  background: #3289b1;
  color: white;
}

@media (max-width: 650px) {
  .research-topic h2 {
    font-size: 1.25em;
  }
}
</style>

<div class="research-page">

<p class="research-intro">
My research in distributed and federated learning focuses on developing
efficient and robust optimization algorithms for settings where data and
computation are distributed across multiple clients. Two important challenges
are reducing communication costs and ensuring reliable learning when some
participants provide corrupted or adversarial updates.
</p>

<p>
I investigate these challenges through two complementary directions:
Byzantine-resilient federated learning and communication-efficient optimization
using Trajectory-Adaptive Error Feedback (TA-EF).
</p>

<figure class="research-figure">
  <img
    src="{{ '/images/distributed-learning-overview.png' | relative_url }}"
    alt="Illustration of federated learning, Byzantine clients, and adaptive error-feedback compression."
    loading="lazy">
  <figcaption>
    Two challenges in distributed optimization: robustness to adversarial
    clients and efficient communication between distributed workers.
  </figcaption>
</figure>

<section class="research-topic" id="byzantine-fl">

<h2>1. Byzantine-Resilient Federated Learning</h2>

<p>
Federated learning enables multiple clients to collaboratively train a model
without sharing their local datasets. However, distributed training becomes
more challenging when client data are heterogeneous or some participants send
malicious or corrupted updates.
</p>

<p>
My work explores Byzantine-resilient optimization methods that aim to maintain
reliable learning in the presence of adversarial clients. I am particularly
interested in aggregation rules, robust optimization algorithms, and the
interaction between robustness and non-independent and identically distributed
(non-IID) data.
</p>

<div class="research-highlight">
<strong>Research questions</strong>
<ul>
  <li>How can distributed optimization tolerate malicious or corrupted client updates?</li>
  <li>How do data heterogeneity and non-IID distributions affect robustness?</li>
  <li>How can robustness guarantees be combined with practical algorithmic efficiency?</li>
</ul>
</div>

<p>
This direction combines theoretical analysis with computational experiments
to understand the strengths and limitations of robust aggregation methods
in federated optimization.
</p>

<div class="research-links">
  <a href="{{ '/publications/' | relative_url }}">Related publications ↗</a>
  <a href="https://github.com/">Code and experiments ↗</a>
</div>

</section>

<section class="research-topic" id="adaptive-ef">

<h2>2. Trajectory-Adaptive Error Feedback</h2>

<p>
Communication is a major bottleneck in distributed optimization. Gradient
compression can reduce the amount of information exchanged between workers,
but aggressive compression can also affect convergence.
</p>

<p>
In my work on <strong>Trajectory-Adaptive Error Feedback (TA-EF)</strong>,
I study communication-efficient optimization methods that adapt compression
to the optimization trajectory. The approach relaxes the uniform contractive
condition commonly used in error-feedback analyses and instead uses a
pointwise relative-error condition.
</p>

<p>
This provides a framework for adapting compression levels during optimization
rather than requiring a fixed compression guarantee at every iteration.
The goal is to improve communication efficiency while retaining rigorous
convergence guarantees.
</p>

<div class="research-highlight">
<strong>Research questions</strong>
<ul>
  <li>How can compression adapt to the behavior of an optimization algorithm?</li>
  <li>Can weaker, trajectory-dependent assumptions provide useful convergence guarantees?</li>
  <li>How can communication savings be balanced against optimization accuracy?</li>
</ul>
</div>

<p>
The work combines theoretical convergence analysis with numerical experiments
to study the trade-offs between compression, communication, and optimization
performance.
</p>

<div class="research-links">
  <a href="{{ '/publications/' | relative_url }}">Related publications ↗</a>
  <a href="https://github.com/">Code and experiments ↗</a>
</div>

</section>

<section class="research-topic" id="related-work">

<h2>Related Publications and Projects</h2>

<p>
For related papers, preprints, and available implementations, visit my
<a href="{{ '/publications/' | relative_url }}">publications page</a>.
Additional project descriptions and code links can be added here as the
research develops.
</p>

</section>

</div>

