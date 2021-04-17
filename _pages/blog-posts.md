---
title: "Blog Posts"
layout: single
permalink: /blog-posts/
---
{% assign posts = site.posts %}

{%- for post in posts -%}
    {%- if post.category == "Blog Post" -%}
        {% include archive-single.html type=entries_layout %}
    {%- endif -%} 
{%- endfor -%}