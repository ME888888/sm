---
layout: default
title: 文章列表
permalink: /posts/
---
<div class="posts-page">
  <div class="posts-list">
    {% for post in site.posts %}
    <div class="post-item">
      <time class="post-date">{{ post.date | date: '%Y年%m月%d日' }}</time>
      <a href="{{ site.baseurl }}{{ post.url }}" class="post-link">{{ post.title }}</a>
    </div>
    {% endfor %}
  </div>
  <!-- Updated: 文章列表包含所有分类 -->
</div>
