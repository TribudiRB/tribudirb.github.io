---
permalink: /aws.html
layout: default
title: AWS
---

{% for post in site.categories.AWS %}
 <li><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}

