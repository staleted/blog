---
layout: page
permalink: /research/
title: Research
description: 
---

Details on my formal publications, research interests, and paper reviews. Note that I publish under my full name, Edward W. Staley. My full publications list can be found on Google Scholar.
<br/>
<hr/>
<br/>

<ul class="post-list">
{% for poem in site.research reversed %}
    <li>
        <h2 style="font-size:48px;"><a class="post-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y' }}</p>
        <p>{{ poem.excerpt  }}</p>
        <br/>
        <hr/>
      </li>
{% endfor %}
</ul>