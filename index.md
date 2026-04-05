---
layout: default
title: "CHINESE POSTPUNK ANTHOLOGY"
---

<ul class="zine-list">
{% for post in site.posts %}
  {% if post.lang == "en" %}
  <li>
    <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
    <div>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </div>
    <p class="post-excerpt">{{ post.excerpt }}</p>
  </li>
  {% endif %}
{% endfor %}
</ul>