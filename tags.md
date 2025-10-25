---
layout: page
title: Tags
permalink: /tags/
---

# Tags

<ul>
  {% assign alltags = site.tags | sort %}
  {% for tag in alltags %}
    <li>
      <a href="/tags/{{ tag[0] | slugify }}/">{{ tag[0] }} ({{ tag[1].size }})</a>
    </li>
  {% endfor %}
</ul>
