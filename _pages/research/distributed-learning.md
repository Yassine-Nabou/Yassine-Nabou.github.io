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

/* HTML-only research illustration */
.fl-diagram {
  margin: 2em 0 2.5em;
  padding: 24px;
  background: #f5f7fb;
  border: 1px solid #dce3ed;
  border-radius: 12px;
  color: #343b46;
}

.fl-diagram * {
  box-sizing: border-box;
}

.fl-diagram-title {
  margin-bottom: 20px;
  text-align: center;
  font-size: 1.15em;
  font-weight: 700;
}

.fl-server {
  max-width: 360px;
  margin: 0 auto;
  padding: 18px;
  text-align: center;
  background: #e2ebfa;
  border: 1px solid #9bb6e0;
  border-radius: 9px;
}

.fl-server strong,
.fl-client strong {
  display: block;
  margin-bottom: 5px;
}

.fl-server small,
.fl-client small {
  display: block;
  line-height: 1.5;
}

.fl-arrows {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  margin: 3px 0;
  color: #5276aa;
  text-align: center;
  font-size: 30px;
  line-height: 1.4;
}

.fl-clients {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 12px;
}

.fl-client {
  min-width: 0;
  padding: 16px 8px;
  text-align: center;
  border: 1px solid;
  border-radius: 9px;
}

.fl-honest {
  background: #e8f5ec;
  border-color: #a5cfb2;
}

.fl-honest strong {
  color: #286b43;
}

.fl-byzantine {
  background: #fff0ed;
  border-color: #e5b2aa;
}

.fl-byzantine strong {
  color: #a33f34;
}

.fl-direction-label {
  margin: 12px 0 20px;
  text-align: center;
  color: #667085;
  font-size: 0.88em;
}

.fl-projects {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 14px;
  margin-top: 20px;
}

.fl-project {
  padding: 17px;
  background: #fff;
  border: 1px solid #dce3ed;
  border-radius: 9px;
}

.fl-project strong {
  display: block;
  margin-bottom: 7px;
  color: #315b91;
}

.fl-project p {
  margin: 0;
  font-size: 0.9em;
  line-height: 1.6;
}

.fl-caption {
  margin-top: 12px;
  color: #64748b;
  font-size: 0.88em;
  text-align: center;
}

@media (max-width: 600px) {
  .fl-diagram {
    padding: 14px;
  }

  .fl-clients {
    gap: 6px;
  }

  .fl-client {
    padding: 12px 4px;
    font-size: 0.84em;
    overflow-wrap: anywhere;
  }

  .fl-projects {
    grid-template-columns: 1fr;
  }

  .research-topic h2 {
    font-size: 1.25em;
  }
}
</style>

<div class="research-page">

<p class="research-intro">
My research in distributed and federated learning focuses on developing efficient and robust optimization algorithms for settings where data and computation are distributed across multiple clients. Two important challenges are reducing communication costs and ensuring reliable learning when some participants provide corrupted or adversarial updates.
</p>

<p>
I investigate these challenges through two complementary directions: Byzantine-resilient federated learning and communication-efficient optimization using Trajectory-Adaptive Error Feedback (TA-EF).
</p>

<div class="fl-diagram">

  <div class="fl-diagram-title">
    Distributed Learning: Two Key Challenges
  </div>

  <div class="fl-server">
    <strong>Central Server</strong>
    <small>Aggregate client updates and distribute the global model</small>
  </div>

  <div class="fl-arrows" aria-hidden="true">
    <div>↙</div>
    <div>↓</div>
    <div>↘</div>
  </div>

  <div class="fl-clients">

    <div class="fl-client fl-honest">
      <strong>Client 1</strong>
      <small>Local data</small>
      <small>Honest update</small>
    </div>

    <div class="fl-client fl-honest">
      <strong>Client 2</strong>
      <small>Local data</small>
      <small>Honest update</small>
    </div>

    <div class="fl-client fl-byzantine">
      <strong>Client 3</strong>
      <small>Potential attacker</small>
      <small>Corrupted update</small>
    </div>

  </div>

  <div class="fl-direction-label">
    Distributed clients create local updates that must be communicated and aggregated.
  </div>

  <div class="fl-projects">

    <div class="fl-project">
      <strong>01 · Byzantine-Resilient Learning</strong>
      <p>
        How can optimization remain reliable when some clients send
        malicious or corrupted updates?
      </p>
    </div>

    <div class="fl-project">
      <strong>02 · Adaptive Error Feedback</strong>
      <p>
        How can adaptive compression reduce communication while
        maintaining optimization accuracy?
      </p>
    </div>

  </div>

</div>

<section class="research-topic" id="byzantine-fl">

<h2>1. Byzantine-Resilient Federated Learning</h2>

<p>
Federated learning enables multiple clients to collaboratively train a model without sharing their local datasets. However, distributed training becomes more challenging when client data are heterogeneous or some participants send malicious or corrupted updates.
</p>

<p>
My work explores Byzantine-resilient optimization methods that aim to maintain reliable learning in the presence of adversarial clients. I am particularly interested in aggregation rules, robust optimization algorithms, and the interaction between robustness and non-independent and identically distributed (non-IID) data.
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
This direction combines theoretical analysis with computational experiments to understand the strengths and limitations of robust aggregation methods in federated optimization.
</p>

<div class="research-links">
<a href="{{ '/publications/' | relative_url }}">Related publications ↗</a>
</div>

</section>

<section class="research-topic" id="adaptive-ef">

<h2>2. Trajectory-Adaptive Error Feedback</h2>

<p>
Communication is a major bottleneck in distributed optimization. Gradient compression can reduce the amount of information exchanged between workers, but aggressive compression can also affect convergence.
</p>

<p>
In my work on <strong>Trajectory-Adaptive Error Feedback (TA-EF)</strong>, I study communication-efficient optimization methods that adapt compression to the optimization trajectory. The approach relaxes the uniform contractive condition commonly used in error-feedback analyses and instead uses a pointwise relative-error condition.
</p>

<p>
This provides a framework for adapting compression levels during optimization rather than requiring a fixed compression guarantee at every iteration. The goal is to improve communication efficiency while retaining rigorous convergence guarantees.
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
The work combines theoretical convergence analysis with numerical experiments to study the trade-offs between compression, communication, and optimization performance.
</p>

<div class="research-links">
<a href="{{ '/publications/' | relative_url }}">Related publications ↗</a>
</div>

</section>

<section class="research-topic" id="related-work">

<h2>Related Publications and Projects</h2>

<p>
For related papers, preprints, and available implementations, visit my
<a href="{{ '/publications/' | relative_url }}">publications page</a>.
Additional project descriptions and code links can be added here as the research develops.
</p>

</section>

</div>
