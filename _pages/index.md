---
title: "Welcome to my blog of failures, mistakes and catastrophes."
layout: tags
permalink: /
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: assets//images//Home_Page_Image.png
  caption: "Photo credit: [**Dariusz Sankowski**](https://unsplash.com/@dariuszsankowski)"
excerpt: "My aim is to help you avoid the same trapings that I encountered in the process of learning drawing, writing fiction and game dev."
---

## Here are some of my most recent posts

{% assign posts = site.posts %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts limit: 5 %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>
---

## Posts sorted by tags