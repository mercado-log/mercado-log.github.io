---
layout: page
title: Posts
permalink: /posts/
---

<div style="max-width: 600px; margin: 0 auto;">
{% assign sorted_posts = site.posts | sort: 'date' %}
{% for post in sorted_posts %}
  <div style="margin-bottom: 1.5rem; padding-bottom: 1.5rem; border-bottom: 1px solid #eee;">
    <span style="color: #828282; font-size: 13px;">{{ post.date | date: "%d/%m/%Y" }}</span><br>
    <a href="{{ post.url }}" style="font-size: 18px; text-decoration: underline;">{{ post.title }}</a>
  </div>
{% endfor %}
</div>
