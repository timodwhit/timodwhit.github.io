---
layout: default
title: Writings
permalink: /writings/
---
<h1>Writings</h1>
<div class="col-1">
  <h2><a href="/writings/personal">Musings</a></h2>
  <ul class="posts">
    {% for post in site.categories.personal %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
</div>

<div class="col-2">
  <h2><a href="/writings/web">Web</a></h2>
  <ul class="posts">
    {% for post in site.categories.web %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
</div>
