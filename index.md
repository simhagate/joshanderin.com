---
layout: default
title: Josh and Erin
---

<div id="posts">

    <ul>
    {% for post in site.posts offset: 0 limit: 10 %}
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

	<hr />

    <center>
        <a href="{{ site.baseurl }}/allposts.html">See More Posts</a>
    </center>

</div>
