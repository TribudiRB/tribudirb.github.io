---
layout: default
title: Home
---
<h1>Interesting facts and useful tips about Programing & Soft Skills</h1>

<h2 class="post-list-heading">Posts</h2>
<ul class="post-list">
{% for post in site.posts %}
    <span class="post-meta">{{ post.date | date_to_long_string: "ordinal", "US"  }}</span>
    <li><a class="post-link" href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
