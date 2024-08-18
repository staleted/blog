---
layout: page
permalink: /projects/
title: Projects
description: Projects
---

<br/>
Lorem ipsum.
<br/>

<ul class="post-list">
{% for poem in site.projects reversed %}
    <li>
        <h2 style="font-size:48px;"><a class="post-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y' }}</p>
        <p>{{ poem.excerpt  }}</p>
        <br/>
        <hr/>
      </li>
{% endfor %}
</ul>