---
title: ""
layout: single
author_profile: false
classes: wide
permalink: /
---

<section class="hero-panel">
  <div class="hero-panel__main">
    <span class="hero-panel__badge">Adithya's learning journal</span>
    <h1>Practical notes on data science, AI, and cloud.</h1>
    <p>
      A cleaner GitHub Pages blog for technical writing, experiments, deployment notes, and project breakdowns.
    </p>
    <div class="hero-panel__actions">
      <a class="btn btn--primary" href="{{ '/blog/' | relative_url }}">Read posts</a>
      <a class="btn btn--light-outline" href="{{ '/about/' | relative_url }}">About me</a>
    </div>
  </div>

  <div class="hero-panel__side">
    <p class="hero-panel__eyebrow">Focus</p>
    <h2>Readable, simple, and deployable.</h2>
    <ul class="hero-panel__list">
      <li>Data science notes and concept explainers</li>
      <li>AI experiments and implementation logs</li>
      <li>Cloud deployment and production workflows</li>
    </ul>
  </div>
</section>

<section class="feature-row">
  <div class="feature-card">
    <span class="feature-card__title">AI</span>
    <span class="feature-card__text">Experiments and workflow notes</span>
  </div>
  <div class="feature-card">
    <span class="feature-card__title">Cloud</span>
    <span class="feature-card__text">Deployment guides and infra learnings</span>
  </div>
  <div class="feature-card">
    <span class="feature-card__title">Data</span>
    <span class="feature-card__text">Projects, notebooks, and practical lessons</span>
  </div>
</section>

<section class="topic-section">
  <h2>What you'll find here</h2>
  <div class="topic-grid">
    <article class="topic-card">
      <strong>Data Science</strong>
      <p>Concept explainers, datasets, notebooks, analysis walkthroughs, and practical project lessons.</p>
    </article>
    <article class="topic-card">
      <strong>Artificial Intelligence</strong>
      <p>Experiments, implementation notes, model workflows, and learning logs around modern AI tools.</p>
    </article>
    <article class="topic-card">
      <strong>Cloud</strong>
      <p>Deployment guides, infrastructure notes, and production-friendly workflows for small projects.</p>
    </article>
  </div>
</section>

<section class="summary-panel">
  <h2>Why this blog exists</h2>
  <p>
    The goal is simple: make technical learning easier to publish and easier to read. Posts are written in Markdown, version-controlled on GitHub, and deployed through GitHub Pages.
  </p>
</section>

<section class="recent-posts">
  <h2>Recent posts</h2>
  <div class="recent-posts__grid">
    {% for post in site.posts limit:3 %}
    <article class="recent-post">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="recent-post__meta">{{ post.date | date: "%B %-d, %Y" }}</p>
      <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
    </article>
    {% endfor %}
  </div>
</section>
