---
title: "Articles"
layout: archive
permalink: /articles/
---
{% assign posts = site.posts %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {%- if post.category == "Article" -%}
        {% include archive-single.html type=entries_layout %}
    {%- endif -%} 
  {% endfor %}
</div>
