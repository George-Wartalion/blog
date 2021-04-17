---
title: "Articles"
layout: single
permalink: /articles/
---
{% assign posts = site.posts %}

{%- for post in posts -%}
    {%- if post.category == "Article" -%}
        {% include archive-single.html type=entries_layout %}
    {%- endif -%} 
{%- endfor -%}