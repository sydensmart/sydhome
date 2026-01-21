---
layout: page
title: Discovery
permalink: /discovery/
---

## List of Study History

<ul>
  {% for item in site.discovery %}
    <li>
      <a href="{{ site.baseurl }}{{ item.url }}">{{ item.title }}</a> - {{ item.date | date: "%Y-%m-%d" }}
    </li>
  {% endfor %}
</ul>
