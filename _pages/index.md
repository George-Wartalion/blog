---
title: "Welcome to my blog of failures, mistakes and catastrophes."
layout: splash
permalink: /
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: assets//images//Temporary_Home_Page_Banner.png
  caption: "Photo credit: [**Dariusz Sankowski**](https://unsplash.com/@dariuszsankowski)"
excerpt: "My aim is to help you avoid the same trapings that I encountered in the process of learning drawing, writeing fiction and reading japanese."
---

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>

{% include paginator.html %}