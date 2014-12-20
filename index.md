---
layout: default
title: Home
---

## Protein
<ul class="posts">
{% for post in site.categories.protein %}
    <li> <a href=".{{ post.url }}">{{ post.title }}</a> </li>
{% endfor %}
</ul>

## Enzyme Assays
<ul class="posts">
{% for post in site.categories.enzyme_assays %}
    <li> <a href=".{{ post.url }}">{{ post.title }}</a> </li>
{% endfor %}
</ul>


