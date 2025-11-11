---
layout: default
title: Home
---

# Welcome to Zero to Hero -> CUDA

Going from a complete beginner in C++ and CUDA to building high performance applications.

## About this blog

I have been wanting to learn CUDA for a while and decided the time to learn is now. The aim is to learn myself and then teach it to everyone who reads the blog. So hopefully, we will all go from complete novices to experts in GPU programming!


## Recent Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

## Learning Resources 
I will add to this section resources I am to cover and anything extra I find along my learning journey: 

- **Books:** *Professional CUDA C Programming*, *Programming Massively Parallel Processors* 
- **Courses:** Elliot Arledge's CUDA course, NVIDIA official training
 