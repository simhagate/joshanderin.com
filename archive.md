---
layout: default
title: Blog Archive
---

# {{ page.title }}

<ul id="post-list">
{% for post in site.posts %}
    <li>
        <small>{{ post.date | date: "%B %d, %Y" }}</small>
        <a href="{{ post.url }}">
            {{ post.title }}
        </a>
    </li>
{% endfor %}
</ul>
