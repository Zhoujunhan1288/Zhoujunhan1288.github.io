---
layout: default
title: Tags
permalink: /tags/
---

<div class="hero">
  <h1>Tags</h1>
  <p>Click a tag to see all related entries.</p>

  <div class="section"></div>

  <p>
    <a class="backbtn" href="{{ '/log/' | relative_url }}">← Back to Research Log</a>
  </p>

  <div class="section"></div>

  {% for tag in site.tags %}
    {% assign tag_name = tag[0] %}
    {% assign tag_posts = tag[1] %}
    <a class="cardbtn" href="{{ '/tag/' | append: tag_name | append: '/' | relative_url }}">
      <div class="head"><span class="badge">#</span>{{ tag_name }}</div>
      <div class="desc">{{ tag_posts | size }} entries</div>
    </a>
  {% endfor %}
</div>
