---
layout: page
icon: fas fa-feather
order: 2
math: true
---

{% for post in site.blog%}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
  <a href="{{ post.url }}">Read More >></a>
{% endfor %}
