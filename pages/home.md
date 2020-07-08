---
layout: default
title: Mark Wetzel | Projects
permalink: /
nav: light
---

<section class="home-hero">
  <div class="pw-container">
    <div class="home-hero-content">
      <p>Hey! I'm <span class="green-text">Mark Wetzel</span>, a UX designer focused on products and problem solving.</p>
      <a class="btn-lrg btn-lrg-dark" href="{{ "/contact/" | relative_url }}">Contact Me</a>
    </div>
  </div>
</section>

<section class="home-projects">
  <div class="pw-container">
    <h3><a name="projects"></a>Projects</h3>
    <div class="home-projects-list">
      {% for item in site.data.projects.list %}
      <div class="home-project">
        <a href="{{ item.url }}" alt="{{ item.title }}">
          <img class="home-project-thumbnail" src="{{ item.thumbnail }}" />
          <h4 class="home-project-title">{{ item.title }}</h4>
          <p class="home-project-description">{{ item.description }}</p>
        </a>
      </div>
      {% endfor %}
    </div>
  </div>
</section>
