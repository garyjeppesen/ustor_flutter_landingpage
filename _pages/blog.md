---
layout: default
title: Blog
permalink: /blog/
---

{% raw %}
<div class="blog-index">
  {% for post in site.posts %}
    <article class="post">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <span class="date">{{ post.date | date: "%B %d, %Y" }}</span>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
{% endraw %}
