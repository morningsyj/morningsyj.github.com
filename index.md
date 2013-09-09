---
layout: page
title: MorningSYJ
tagline: 记录学习和生活的点滴
---

## 前端姑且随便搞搞，国庆节再来装修:)



## 所有文章

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

