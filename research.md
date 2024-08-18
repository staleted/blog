---
layout: page
permalink: /research/
title: Research
description: Research
---

<ul class="post-list">
{% for poem in site.research reversed %}
    <li>
        <h2><a class="post-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y — %H:%M' }}</p>
        <p>{{ poem.excerpt  }}</p>
        <br/>
        <hr/>
      </li>
{% endfor %}
</ul>