---
layout: default
title: Blog
permalink: /blog/
---

<div class="home">

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
          <div>{{ post.summary }}</div>
        </h2>
      </li>
    {% endfor %}
  </ul>

</div>