---
layout: default
title: "CHINESE POSTPUNK ANTHOLOGY"
---
<div class="zine">
<ul class="zine-list">
{% for post in site.posts %}
  <li>
    <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
    <div class="post-title"><a href="{{ post.url }}">{{ post.title }}{% if post.lang %} — {{ post.lang }}{% endif %}</a></div>
    <p class="post-excerpt">{{ post.excerpt }}</p>
  </li>
{% endfor %}
</ul>
</div>