---
layout: page
permalink: /implementations/
title: Implementations
description: Items that don't belong in the other categories.
---

<ul class="post-list">
    {% for post in paginator.other %}
      <li>
        <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
        <p>{{ post.excerpt  }}</p>
        <br/>
        <hr/>
      </li>
    {% endfor %}
</ul>