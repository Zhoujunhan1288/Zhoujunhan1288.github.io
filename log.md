---
layout: default
title: 研究日志
permalink: /log/
---

# 研究日志
按年 → 月 → 日浏览。

{% assign posts_by_year = site.posts | group_by_exp:"post", "post.date | date: '%Y'" %}

{% for year in posts_by_year %}
  <div class="section"></div>
  <h2>{{ year.name }}</h2>

  {% assign posts_by_month = year.items | group_by_exp:"post", "post.date | date: '%m'" %}
  {% for month in posts_by_month %}
    <h3>{{ month.name }} 月</h3>
    {% for post in month.items %}
      <div class="post-item">
        <a href="{{ post.url | relative_url }}">{{ post.date | date: "%m-%d" }} · {{ post.title }}</a>
        <div class="post-meta">{{ post.categories | join: ", " }}</div>
      </div>
    {% endfor %}
  {% endfor %}
{% endfor %}
