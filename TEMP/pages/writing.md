---
layout: page
title: Writing
permalink: /writing/
---

<div class="writing-list">
  {% for post in site.posts %}
    <div class="writing-list-post">
      {% assign date_format = site.minima.date_format | default: "%Y %b %-d" %}
      <span class="writing-list-post-date">{{ post.date | date: date_format }}</span>
      <p class="writing-list-post-title">
        <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </p>
    </div>
  {% endfor %}
</div>
