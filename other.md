---
layout: page
permalink: /other/
title: Other
description: Items that don't belong in the other categories.
---

<ul class="post-list">
{% for poem in site.other reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>