---
layout: page
title: explore
permalink: /explore/
---

## 관심영역에 대한 지속적 탐험 목록

<ul>
  {% for item in site.explore %}
    <li>
      <a href="{{ site.baseurl }}{{ item.url }}">{{ item.title }}</a> - {{ item.date | date: "%Y-%m-%d" }}
    </li>
  {% endfor %}
</ul>
