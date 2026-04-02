---
layout: home 
title: "CHINESE POSTPUNK ANTHOLOGY"
---


<div class="zine">


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

    {% include footer.html %}  