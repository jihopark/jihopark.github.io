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
      <li><a href="#{{ tag_name | slugify }}">{{ tag_name }} ({{ tag[1].size }})</a></li>
    {% endfor %}
  </ul>

  {% for tag in tags %}
    {% assign tag_name = tag[0] %}
    {% assign posts = tag[1] %}
    <h3 id="{{ tag_name | slugify }}">{{ tag_name }}</h3>
    <ul>
    {% for post in posts %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <small>{{ post.date | date_to_string }}</small>
      </li>
    {% endfor %}
    </ul>
  {% endfor %}
</div>


