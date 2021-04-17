---
title: "Reviews"
layout: single
permalink: /reviews/
---
{% assign posts = site.posts %}

{%- for post in posts -%}
    {%- if post.category == "Review" -%}
        {% include archive-single.html type=entries_layout %}
    {%- endif -%} 
{%- endfor -%}