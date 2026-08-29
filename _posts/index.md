# Blog

Here are my latest posts:

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})

{{ post.excerpt }}

*{{ post.date | date: "%B %d, %Y" }}*

{% endfor %}