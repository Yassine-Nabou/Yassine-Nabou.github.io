---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
.home-page {
  max-width: 1000px;
  margin: 0 auto;
  line-height: 1.7;
}

.home-hero {
  padding: 0.5em 0 2em;
}

.home-hero h1 {
  font-size: 1.8em;
  line-height: 1.3;
  margin: 0 0 0.65em;
  letter-spacing: -0.02em;
}

.home-lead {
  font-size: 1.08em;
  margin-bottom: 1.4em;
}

.home-position {
  display: flex;
  align-items: flex-start;
  gap: 1em;
  padding: 1.25em 1.4em;
  margin: 1.8em 0 2.8em;
  border: 1px solid #dce7ef;
  border-left: 4px solid #3289b1;
  border-radius: 7px;
  background: rgba(50, 137, 177, 0.045);
}

.home-position-icon {
  flex-shrink: 0;
  font-size: 1.5em;
  line-height: 1.4;
}

.home-position p {
  margin: 0.15em 0;
}

.home-position-label {
  font-size: 0.82em;
  text-transform: uppercase;
  letter-spacing: 0.07em;
  color: #64748b;
  font-weight: 700;
}

.home-section {
  margin: 2.7em 0;
}

.home-section h2 {
  font-size: 1.5em;
  margin-bottom: 0.35em;
  padding-bottom: 0.45em;
  border-bottom: 1px solid #e5e7eb;
}

.home-section-intro {
  margin-bottom: 1.3em;
}

.home-research-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 1em;
  margin-top: 1.4em;
}

.home-research-card {
  display: block;
  padding: 1.2em;
  border: 1px solid #e1e7ed;
  border-radius: 8px;
  color: inherit !important;
  text-decoration: none !important;
  transition: border-color 0.2s ease, transform 0.2s ease,
              box-shadow 0.2s ease;
}

.home-research-card:hover,
.home-research-card:focus {
  border-color: #8bbbd1;
  transform: translateY(-2px);
  box-shadow: 0 4px 14px rgba(30, 70, 90, 0.08);
}

.home-research-card h3 {
  font-size: 1.08em;
  margin: 0 0 0.5em;
  color: #3289b1;
}

.home-research-card p {
  font-size: 0.95em;
  margin: 0;
}

.home-card-icon {
  font-size: 1.5em;
  margin-bottom: 0.45em;
  line-height: 1.3;
}

.home-card-footer {
  display: block;
  margin-top: 0.8em;
  color: #3289b1;
  font-size: 0.88em;
  font-weight: 600;
}

.home-links {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1em;
  margin: 1.4em 0 2em;
}

.home-link-card {
  display: block;
  padding: 1.1em;
  border: 1px solid #e1e7ed;
  border-radius: 8px;
  text-decoration: none !important;
  transition: border-color 0.2s ease, transform 0.2s ease;
}

.home-link-card:hover,
.home-link-card:focus {
  border-color: #8bbbd1;
  transform: translateY(-2px);
}

.home-link-card strong {
  display: block;
  margin-bottom: 0.25em;
}

.home-link-card span {
  display: block;
  font-size: 0.88em;
  line-height: 1.5;
  color: #64748b;
}

.home-phd {
  padding-left: 1.1em;
  border-left: 3px solid #dce7ef;
  margin: 1.4em 0;
}

.home-phd p {
  margin: 0.35em 0;
}

.home-thesis-link {
  display: inline-block;
  padding: 0.1em 0.55em;
  border: 1px solid #dce3ec;
  border-radius: 4px;
  font-size: 0.88em;
  text-decoration: none !important;
}

@media (max-width: 650px) {
  .home-hero h1 {
    font-size: 1.8em;
  }

  .home-research-grid,
  .home-links {
    grid-template-columns: 1fr;
  }

  .home-position {
    padding: 1em;
  }
}
</style>

<div class="home-page">

  <section class="home-hero">
    <h1>Welcome to my personal webpage</h1>

    <p class="home-lead">
      I am a researcher working at the intersection of mathematical
      optimization and machine learning. My work focuses on the development,
      theoretical analysis, and numerical implementation of algorithms for
      convex and nonconvex problems. I am particularly interested in designing
      efficient, adaptive, and scalable optimization methods for challenging
      problems in scientific computing and modern AI.
    </p>
  </section>

  <section class="home-position">
    <div class="home-position-icon" aria-hidden="true">🎓</div>
    <div>
      <p class="home-position-label">Current Position</p>
      <p><strong>Postdoctoral Researcher</strong></p>
      <p>
        Department of Mathematics and Statistics,
        <a href="https://www.helsinki.fi/en">University of Helsinki</a>, Finland
      </p>
      <p>
        Working with <a href="https://tuomov.iki.fi">Tuomo Valkonen</a>.
      </p>
    </div>
  </section>

  <section class="home-section" id="research">
    <h2>Research Interests</h2>
    <p class="home-section-intro">
      My research combines optimization theory, algorithm design, and
      computational methods. Select a topic to learn more about my work,
      related publications, and research projects.
    </p>

    <div class="home-research-grid">

      <a class="home-research-card"
         href="{{ '/research/optimization/' | relative_url }}">
        <div class="home-card-icon" aria-hidden="true">∇</div>
        <h3>Optimization Algorithms</h3>
        <p>
          Convex and nonconvex optimization, nonsmooth composite problems,
          constrained optimization, and second- and higher-order methods.
        </p>
        <span class="home-card-footer">Explore this topic ↗</span>
      </a>

      <a class="home-research-card"
         href="{{ '/research/machine-learning/' | relative_url }}">
        <div class="home-card-icon" aria-hidden="true">◇</div>
        <h3>Optimization for Machine Learning</h3>
        <p>
          Optimization methods for machine learning and AI, with an emphasis
          on algorithmic efficiency, adaptivity, and theoretical guarantees.
        </p>
        <span class="home-card-footer">Explore this topic ↗</span>
      </a>

      <a class="home-research-card"
         href="{{ '/research/distributed-learning/' | relative_url }}">
        <div class="home-card-icon" aria-hidden="true">⇄</div>
        <h3>Distributed and Federated Learning</h3>
        <p>
          Communication-efficient optimization, distributed algorithms,
          and robust learning in heterogeneous and adversarial environments.
        </p>
        <span class="home-card-footer">Explore this topic ↗</span>
      </a>

      <a class="home-research-card"
         href="{{ '/research/inverse-problems/' | relative_url }}">
        <div class="home-card-icon" aria-hidden="true">⌘</div>
        <h3>Inverse Problems and Scientific Computing</h3>
        <p>
          Optimization methods for inverse problems, dynamic systems,
          and large-scale computational applications.
        </p>
        <span class="home-card-footer">Explore this topic ↗</span>
      </a>

    </div>
  </section>

  <section class="home-section" id="education">
    <h2>Academic Background</h2>

    <div class="home-phd">
      <p>
        I received my Ph.D. in Automatic Control and Systems Engineering
        in May 2024, under the supervision of
        <a href="https://acse.pub.ro/index.php/en/ion-necoara/">Ion Necoara</a>,
        at the National University of Science and Technology POLITEHNICA Bucharest.
      </p>
      <p>
        My doctoral research was conducted within the Marie Skłodowska-Curie
        <a href="https://trade-opt-itn.eu">TraDE-OPT H2020 Innovative Training Network</a>,
        where I was an Early Stage Researcher (ESR10).
      </p>
      <p>
        <a class="home-thesis-link"
           href="{{ '/files/Yassine_nabou_PHD.pdf' | relative_url }}"
           target="_blank" rel="noopener">
          Read my Ph.D. thesis (PDF) ↗
        </a>
        &nbsp;
        <a href="{{ '/cv-yassine/' | relative_url }}">Full academic CV ↗</a>
      </p>
    </div>
  </section>
</div>
