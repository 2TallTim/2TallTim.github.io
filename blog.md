---
layout: collection
collection: posts
entries_layout: grid
classes: wide
sort_by: date
sort_order: reverse
no_header: true
title: Blog Posts
---

{% unless site[page.collection][0] %}
<h1>Whoops, nothing here!</h1>
{% endunless %}
