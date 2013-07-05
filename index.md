---
layout: default
title: Josh and Erin
---

<div id="posts">

    <ul>
    {% for post in site.posts %}
        <li>
            <h2>
            <a href="{{ post.url }}">
                {{ post.title }}
            </a>
            <small>
                {{ post.date | date: "%B %d, %Y" }}
            </small>
            </h2>
            {{ post.content }}
        </li>
    {% endfor %}
    </ul>

</div>
