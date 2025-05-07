---
layout: default
title: Aspirantes
permalink: /blog/
---

<div style="margin-bottom: 2rem;">
  <a href="/">← Return to Home</a>
</div>

<article class="post">
  <h1 class="post-title">{{ page.title }}</h1>
  <div class="post-content">
    <ul>
      {% assign sorted_posts = site.posts | sort: 'title' %}
      {% for post in sorted_posts %}
        <li>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </li>
      {% endfor %}
    </ul>
  </div>
</article> 