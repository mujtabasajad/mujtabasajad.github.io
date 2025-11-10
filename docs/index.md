---
layout: default
title: Home
---

# Welcome to Zero to Hero -> CUDA

Going from a complete beginner in C++ and CUDA to building high performance applications.

## Recent Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
