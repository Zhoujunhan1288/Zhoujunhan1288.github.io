---
layout: default
title: Research Log
permalink: /log/
---

<div class="hero">
  <h1>Research Log</h1>
  <p>
    This is not a daily diary.  
    Entries are written when something meaningful happens:
    an idea, an experiment milestone, a failure analysis, or a theoretical insight.
  </p>
</div>

<div class="section"></div>

## Browse by Year

<div class="year-grid">
  <a class="year-card" href="{{ '/log/2026/' | relative_url }}">2026</a>
  <a class="year-card" href="{{ '/log/2027/' | relative_url }}">2027</a>
  <a class="year-card" href="{{ '/log/2028/' | relative_url }}">2028</a>
</div>

<div class="section"></div>

## Recent Entries

{% assign recent = site.posts | slice: 0, 5 %}

{% for post in recent %}
<div class="post-item">
  <a href="{{ post.url | relative_url }}">
    <strong>{{ post.date | date: "%Y-%m-%d" }} · {{ post.title }}</strong>
  </a>
  <div class="post-meta">
    {% if post.type %}<strong>{{ post.type }}</strong>{% endif %}
    {% if post.tags %}
      ·
      {% for t in post.tags %}
        <a class="tag" href="{{ '/tag/' | append: t | append: '/' | relative_url }}">#{{ t }}</a>
      {% endfor %}
    {% endif %}
  </div>
</div>
{% endfor %}

<div class="section"></div>

<p>
  <a class="backbtn" href="{{ '/tags/' | relative_url }}">Browse by Tags →</a>
</p>
