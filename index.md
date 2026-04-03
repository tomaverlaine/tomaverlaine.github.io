---
layout: default
title: "CHINESE POSTPUNK ANTHOLOGY"
---
<div class="zine">
<ul class="zine-list">
  {% for post in site.posts %}
* {{ post.date | date: "%Y-%m-%d" }}
  {% if post.lang == "ja" %}[JP]{% elsif post.lang == "en" %}[EN]{% elsif post.lang == "zh" %}[ZH]{% endif %}
  [{{ post.title }}]({{ post.url }})

  {{ post.excerpt }}
{% endfor %}
</ul>
</div>