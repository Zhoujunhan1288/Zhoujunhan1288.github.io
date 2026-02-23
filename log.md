---
layout: default
title: Research Log
permalink: /log/
---

# Research Log

This is my research log (not a daily diary). Entries are written when something meaningful happens: an idea, a breakthrough, a failure analysis, or an experiment milestone.

<div class="section"></div>

## Browse by Year

<ul class="list">
  <li><a href="{{ '/log/2026/' | relative_url }}">2026</a></li>
  <li><a href="{{ '/log/2027/' | relative_url }}">2027</a></li>
  <li><a href="{{ '/log/2028/' | relative_url }}">2028</a></li>
</ul>

<div class="section"></div>

## Recent Entries

{% assign recent = site.posts | slice: 0, 10 %}
{% for post in recent %}
  <div class="post-item">
    <a href="{{ post.url | relative_url }}">{{ post.date | date: "%Y-%m-%d" }} · {{ post.title }}</a>
    <div class="post-meta">
      {% if post.type %}<strong>{{ post.type }}</strong>{% endif %}
      {% if post.tags and post.tags.size > 0 %}
        ·
        {% for t in post.tags %}
          <a href="{{ '/tag/' | append: t | append: '/' | relative_url }}">#{{ t }}</a>{% unless forloop.last %} {% endunless %}
        {% endfor %}
      {% endif %}
    </div>
  </div>
{% endfor %}

<div class="section"></div>

## Tags

<a href="{{ '/tags/' | relative_url }}">Browse all tags →</a>
