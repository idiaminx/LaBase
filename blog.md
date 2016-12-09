---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
title: Blog
permalink: /blog
---

<h1 class="page-heading">Posts</h1>

<!--{{ content }}-->

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | relative_url }}#disqus_thread">{{ post.title | escape }}</a><h4>{{ content.excerpt | default: post.description | strip_html | normalize_whitespace | truncate: 160 | escape }}</h4>
      </h2>
    </li>
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p><br><br>
