---
layout: cinematic-page
title: Blog
subtitle: "Real knowledge is to know the extent of one's ignorance. — Confucius"
cover: false
menu: true
order: 5
---

{% if site.posts.size > 0 %}
<div class="post-list">
  {% for post in site.posts %}
  <a class="post-item" href="{{ post.url }}">
    <div class="post-date">{{ post.date | date: "%B %d, %Y" }}</div>
    <div class="post-title">{{ post.title }}</div>
    <div class="post-excerpt">{{ post.excerpt | strip_html | truncate: 200 }}</div>
    {% if post.tags.size > 0 %}
    <div class="post-tags">
      {% for tag in post.tags %}
      <span class="post-tag">{{ tag }}</span>
      {% endfor %}
    </div>
    {% endif %}
  </a>
  {% endfor %}
</div>
{% else %}
<div class="empty-state">No posts yet.</div>
{% endif %}

<audio autoplay loop> <source src="/assets/audio/sleeping_lotus.mp3" type="audio/mp3"> </audio>
