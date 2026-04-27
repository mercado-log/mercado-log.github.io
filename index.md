---
layout: default
---

<style>
.post-list {
  max-width: 600px;
  margin: 0 auto;
}
.post-list li {
  border-bottom: 1px solid #eee;
  padding-bottom: 1.5rem;
  margin-bottom: 1.5rem;
}
.post-list a {
  text-decoration: underline;
}
</style>

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><br>
      <small>{{ post.date | date: "%d/%m/%Y" }}</small>
    </li>
  {% endfor %}
</ul>
