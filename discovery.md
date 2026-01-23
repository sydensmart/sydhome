---
layout: page
title: Discovery
permalink: /discovery/
---

## List of Study History
이곳은 디지털 혁신과 비즈니스 전략, 그리고 기술적 발견을 기록하는 공간입니다.  
2026년 AI 비즈니스 생태계의 근본적인 변화를 분석하고 기업이 취해야 할 전략적 포지션을 제안합니다.

{% for category in site.data.discovery_categories %}
  <div class="category-section" style="margin-bottom: 30px;">
    <h2 style="border-bottom: 2px solid #eee; padding-bottom: 5px;">{{ category.name }}</h2>
    <p style="color: #666; font-style: italic;">{{ category.description }}</p>
    
    <ul>
      {% assign category_posts = site.discovery | where: "category", category.id %}
      {% for item in category_posts %}
        <li>
          <a href="{{ site.baseurl }}{{ item.url }}">{{ item.title }}</a> 
          <span style="color: #999; font-size: 0.8em;">- {{ item.date | date: "%Y-%m-%d" }}</span>
        </li>
      {% else %}
        <li style="color: #ccc; list-style: none;">작성된 글이 아직 없습니다.</li>
      {% endfor %}
    </ul>
  </div>
{% endfor %}
