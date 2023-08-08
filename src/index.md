---
layout: "base.njk"
---

This is a simple example of building a blog with 11ty and how to deploy it to Github pages via Github Actions.

{% for post in collections.posts %}
- {{ post.data.date }}: [{{ post.data.title }}]({{ post.url }})
{% endfor %}

