---
layout: page
title: "Blog"
---

Ce blog rassemble des billets ponctuels sur l’IA, la recherche, l’enseignement  
et quelques projets personnels.

<ul>
  {% assign posts_fr = site.posts | where: "lang", "fr" %}
  {% for post in posts_fr %}
    <li>
      <span>{{ post.date | date: "%Y-%m-%d" }}</span>
      &nbsp;—&nbsp;
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

