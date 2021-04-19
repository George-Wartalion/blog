---
title: "Articles"
layout: splash
permalink: /articles/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: assets//images//Article_Banner.png
  caption: "Photo credit: [**Patrick Tomasso**](https://unsplash.com/@impatrickt)"
excerpt: "This page is for my long form articles, with which I hope to elaborate and expand my ideas."
---
## Recent Articles

{% assign posts = site.posts %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% if post.category == "Article" %}
        {% include archive-single.html type=entries_layout %}
    {% endif %} 
  {% endfor %}
</div>
