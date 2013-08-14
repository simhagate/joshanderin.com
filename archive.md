---
layout: default
title: Blog Archive
---

# {{ page.title }}

<ul>
{% for post in site.posts %}
    <li>
        <small>{{ post.date | date: "%m/%d/%y" }}</small>
        <a href="{{ post.url }}">
            {{ post.title }}
        </a>
    </li>
{% endfor %}
</ul>
