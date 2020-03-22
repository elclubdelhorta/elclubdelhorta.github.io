---
layout: page
title : Portfolio
permalink: /portfolio/
subtitle: "Projects I am working on"
feature-img: "assets/img/pexels/computer.jpeg"
tags: [Archive]
pagination:
  enabled: true
---
{% for post in site.posts %}
<article>
<h2> entrada
<a href="{{ post.url }}">
{{ post.title }}
</a>
</h2>
<time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
{{ post.content }}
</article>
{% endfor %}

