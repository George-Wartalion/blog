---
title: "Blog Posts"
layout: tags
permalink: /blog-posts/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: assets//images//Blog_Banner.png
  caption: "Photo credit: [**Daria Obymaha**](https://www.pexels.com/@dariaobymaha)"
excerpt: "This page is for my short form and more personal posts, in which I will show parts of my processes and other things that I couldn't put in an article."
---
## Recent Blog Posts
---

{% assign posts = site.posts %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% if post.category == "Blog Post" %}
        {% include archive-single.html type=entries_layout %}
    {% endif %} 
  {% endfor %}
</div>
---

## Blog Posts sorted by tag
---