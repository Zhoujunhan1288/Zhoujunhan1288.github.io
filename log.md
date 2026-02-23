---
layout: default
title: 研究日志
permalink: /log/
---

# 研究日志

选择年份 → 月份 → 具体日期。

---

{% assign posts_by_year = site.posts | group_by_exp:"post", "post.date | date: '%Y'" %}

{% for year in posts_by_year %}
  <h2>{{ year.name }}</h2>

  {% assign posts_by_month = year.items | group_by_exp:"post", "post.date | date: '%m'" %}

  {% for month in posts_by_month %}
    <h3>{{ month.name }} 月</h3>

    <ul class="list">
      {% for post in month.items %}
        <li>
          <a href="{{ post.url | relative_url }}">
            {{ post.date | date: "%m-%d" }} · {{ post.title }}
          </a>
        </li>
      {% endfor %}
    </ul>
  {% endfor %}

{% endfor %}
