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

    <!-- カテゴリ → タグ をカンマ区切りで表示 -->
    {% if post.categories.size > 0 or post.tags.size > 0 %}
      <p class="post-terms">
        {% for term in post.categories %}
          <span class="term">{{ term }}</span>{% unless forloop.last and post.tags.size == 0 %}, {% endunless %}
        {% endfor %}
        {% for term in post.tags %}
          <span class="term">{{ term }}</span>{% unless forloop.last %}, {% endunless %}
        {% endfor %}
      </p>
    {% endif %}

  </li>
  {% endif %}
{% endfor %}
</ul>