---
permalink: /other.html
layout: default
title: Home
---

<h2>Topics by Post Count</h2>
<ul>
{% assign categories_list = site.categories %}
    {% if categories_list.first[0] == null %}
        {% for category in categories_list %}
        {% endfor %}
    {% else %}
        {% for category in categories_list != 'unwantedcategory' %}
            <a href="/topics/#{{ category[0] | url_escape | site_url }}">{{ category[0] | camelcase }} ({{ category[1].size }})</a> |
        {% endfor %}
    {% endif %}
{% assign categories_list = nil %}
</ul>

