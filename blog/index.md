---
layout: page
title: 博客
permalink: /blog/
---

# 我的博客文章

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h2>
        <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h2>
      <p class="post-meta">{{ post.date | date: "%Y年%m月%d日" }}</p>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url | relative_url }}">阅读更多</a>
    </li>
  {% endfor %}
</ul> 