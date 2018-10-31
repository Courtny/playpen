---
layout: page
title: playpen - the danger zone
tagline: A simple website for playing with stuff
description: A place for playing
---

[Github Pages](https://pages.github.com) provide a simple way to make a
website using
[Markdown](https://daringfireball.net/projects/markdown/) and
[git](https://git-scm.com).
which is great for _messing around, man._

{% for post in site.posts %}
<article>
  <h2>
    <a href="{{ post.url }}">
      {{ post.title }}
    </a>
  </h2>
  <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
  {{ post.content }}
</article>
{% endfor %}
