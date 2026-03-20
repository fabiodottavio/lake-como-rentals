---
title: Blog
description: Guides, inspiration and local tips for Lake Como
layout: page
---

<div class="blog-list">
  {% for post in site.posts %}
  <article class="blog-row">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncate: 180 }}</p>
  </article>
  {% endfor %}
</div>
