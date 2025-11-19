---
layout: page
title: "Blog"
---

This blog hosts occasional posts about AI, research, teaching, and side projects.

<ul>
  {% assign posts_en = site.posts | where: "lang", "en" %}
  {% for post in posts_en %}
    <li>
      <span>{{ post.date | date: "%Y-%m-%d" }}</span>
      &nbsp;—&nbsp;
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

