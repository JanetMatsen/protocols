---
layout: default
title: Home
---

## Purification
<ul class="posts">
{% for post in site.categories.purification %}
    <li> <a href=".{{ post.url }}">{{ post.title }}</a> </li>
{% endfor %}
</ul>

