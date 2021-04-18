---
title: "Reviews"
layout: tags
permalink: /reviews/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: assets//images//Review_Banner.png
  caption: "Photo credit: [**Ian Dooley**](https://unsplash.com/@sadswim)"
excerpt: "As the name implies, this page is for reviews of a plethora of things."
---
## Recent Review
---

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts limit: 5 %}
    {% if post.category == "Review" %}
        {% include archive-single.html type=entries_layout %}
    {% endif %} 
  {% endfor %}
</div>

---

## Reviews sorted by tag
---