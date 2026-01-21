---
layout: page
title: Discovery
permalink: /discovery/
---

## 학습 기록 목록

<ul>
  {% for item in site.discovery %}
    <li>
      <a href="{{ site.baseurl }}{{ item.url }}">{{ item.title }}</a> - {{ item.date | date: "%Y-%m-%d" }}
    </li>
  {% endfor %}
</ul>
