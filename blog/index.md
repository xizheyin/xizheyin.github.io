---
layout: page
title: blog
permalink: /blog/
---

## My blog

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h3>
        <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h3>
      <p class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</p>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url | relative_url }}">read more</a>
    </li>
  {% endfor %}
</ul> 