---
layout: default
title: Tags
permalink: /tags/
---

# Tags

**posts:** {{ site.posts | size }}  
**tags:** {{ site.tags | size }}

<div class="section"></div>

{% for tag in site.tags %}
  {% assign tag_name = tag[0] %}
  {% assign tag_posts = tag[1] %}
  <div class="post-item">
    <strong>#{{ tag_name }}</strong>
    <div class="post-meta">({{ tag_posts | size }})</div>
  </div>
{% endfor %}
