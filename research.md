---
layout: page
permalink: /research/
title: Research
description: Research
---

<ul class="post-list">
    {% for post in paginator.research %}
      <li>
        <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
        <p>{{ post.excerpt  }}</p>
        <br/>
        <hr/>
      </li>
    {% endfor %}
</ul>