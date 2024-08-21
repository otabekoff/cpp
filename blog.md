---
layout: default
title: Blog
permalink: /blog/
---

# Blog

Welcome to my blog! Here are some of my latest articles:

<div class="blog-posts">
  {% for post in site.posts %}
    <div class="card">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
      <a href="{{ post.url }}" class="read-more">Read More</a>
    </div>
  {% endfor %}
</div>
