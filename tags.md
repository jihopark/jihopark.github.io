---
layout: page
title: Tags
permalink: /tags/
---

<div class="tags">
  {% assign tags = site.tags | sort %}
  <h2>All Tags</h2>
  <ul class="tag-list">
    {% for tag in tags %}
      {% assign tag_name = tag[0] %}
      <li><a href="/tag/{{ tag_name | slugify }}/">{{ tag_name }} ({{ tag[1].size }})</a></li>
    {% endfor %}
  </ul>

  {% for tag in tags %}
    {% assign tag_name = tag[0] %}
    {% assign posts = tag[1] %}
    <div class="tag-section" id="{{ tag_name | slugify }}">
      <h3><a href="/tag/{{ tag_name | slugify }}/">{{ tag_name }}</a></h3>
    </div>
  {% endfor %}
</div>


