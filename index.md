---
layout: default
---

# 환영합니다!

안녕하세요! 제 블로그에 오신 것을 환영합니다.

## 최근 글

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span>{{ post.date | date: "%Y년 %m월 %d일" }}</span>
    </li>
  {% endfor %}
</ul>
