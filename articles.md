---
layout: article
permalink: /articles/
---

Looking for something? You may find it here.

{% for category in site.categories %}
  <h5>{{ category[0] }}</h5>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}