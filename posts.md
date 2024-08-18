---
layout: page
permalink: /blog/
title: Blog
description: All my posts, in one list.
---

All my posts end up here. They are also split out into categories: Research (details on my publications and reviews of papers I find interesting), Projects (things I work on that are not papers), and Other (everything else).

<ul class="post-list">
{% for poem in site.posts reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>