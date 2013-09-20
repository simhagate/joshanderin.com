---
layout: default
title: All Posts
---

<div id="posts">

    <h1>All Posts</h1>

    <ul>
    {% for post in site.posts %}
        <li>
            <div id="post-header">
            <h2>
            <small class="pull-right">
                {{ post.date | date: "%B %d, %Y" }}
            </small>
            <a href="{{ post.url }}">
                {{ post.title }}
            </a>
            <small>
                by {{ post.author }}
            </small>
            </h2>
            </div>

            {{ post.content }}

        </li>
    {% endfor %}
    </ul>

</div>
