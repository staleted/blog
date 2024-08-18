---
layout: page
permalink: /blog/
title: Blog
description: All my posts, in one list.
---

All my posts end up here. They are also split out into categories: Research (details on my publications and reviews of papers I find interesting), Projects (things I work on that are not papers), and Other (everything else).

<ul class="post-list">
    {% for post in paginator.posts %}
      <li>
        <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
        <p>{{ post.description }}</p>
        <br/>
        <hr/>
      </li>
    {% endfor %}
</ul>