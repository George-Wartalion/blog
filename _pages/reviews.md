---
title: "Reviews"
layout: archive
permalink: /reviews/
---
{% assign posts = site.posts %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {%- if post.category == "Review" -%}
        {% include archive-single.html type=entries_layout %}
    {%- endif -%} 
  {% endfor %}
</div>
