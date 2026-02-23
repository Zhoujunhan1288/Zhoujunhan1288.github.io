---
layout: default
title: Tags
permalink: /tags/
---

# Tags

Click a tag to see all related entries.

<div class="section"></div>

{% assign tags = site.tags | sort %}
<ul class="list">
  {% for tag in tags %}
    {% assign tag_name = tag[0] %}
    {% assign tag_posts = tag[1] %}
    <li>
      <a href="{{ '/tag/' | append: tag_name | append: '/' | relative_url }}">#{{ tag_name }}</a>
      <span class="muted">({{ tag_posts.size }})</span>
    </li>
  {% endfor %}
</ul>
