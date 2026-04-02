---
layout: home 
title: "CHINESE POSTPUNK ANTHOLOGY"
---

<div class="zine">

<h1 class="site-title">CHINESE POSTPUNK ANTHOLOGY</h1>

<p class="intro">
Notes on Chinese indie rock, local scenes, and the conditions that shape them.
</p>

<ul class="zine-list">
  {% for post in site.posts %}
  <li>
    <span class="date">{{ post.date | date: "%Y-%m-%d" }}</span>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <p class="excerpt">{{ post.excerpt }}</p>
  </li>
  {% endfor %}
</ul>

</div>