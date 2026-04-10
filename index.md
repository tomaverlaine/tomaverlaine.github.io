---
layout: default
title: "CHINESE POSTPUNK ANTHOLOGY"
---

<h2>Texts</h2>
<ul class="zine-list">
{% for post in site.posts %}
  {% if post.lang == "en" and post.categories contains "texts" %}
  <li>
    <p>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </p>
    <p class="post-summary">{{ post.summary }}</p>
  </li>
  {% endif %}
{% endfor %}
</ul>


<h2>Features</h2>
<ul class="zine-list">
{% for post in site.posts %}
  {% if post.lang == "en" and post.categories contains "features" %}
  <li>
    <p>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </p>
    <p class="post-summary">{{ post.summary }}</p>
  </li>
  {% endif %}
{% endfor %}
</ul>


<h2>Interviews</h2>
<ul class="zine-list">
{% for post in site.posts %}
  {% if post.lang == "en" and post.categories contains "interviews" %}
  <li>
    <p>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </p>
    <p class="post-summary">{{ post.summary }}</p>
  </li>
  {% endif %}
{% endfor %}
</ul>


<h2>Lists</h2>
<ul class="zine-list">
{% for post in site.posts %}
  {% if post.lang == "en" and post.categories contains "lists" %}
  <li>
    <p>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </p>
    <p class="post-summary">{{ post.summary }}</p>
  </li>
  {% endif %}
{% endfor %}
</ul>