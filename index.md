---
layout: default
title: "CHINESE POSTPUNK ANTHOLOGY"
---
<p>Chinese Postpunk Anthology collects materials documenting independent music scenes across China.</p>

<h2>Texts</h2>
<ul class="zine-list">
{% for post in site.posts %}
  {% if post.lang == "en" and post.categories contains "texts" %}
  <li>
    <div>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </div>
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
    <div>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </div>
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
    <div>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </div>
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
    <div>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </div>
    <p class="post-summary">{{ post.summary }}</p>
  </li>
  {% endif %}
{% endfor %}
</ul>