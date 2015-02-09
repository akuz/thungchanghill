---
layout: page
title: 
permalink: /blog/
---

{% for post in site.posts %}
<div class="page-header">
  <h4><span class="label label-default">{{ post.date | date: "%b %-d, %Y" }}</span></h4>
  <h1><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h1>
</div>
{% endfor %}

<p class="rss-subscribe">Subscribe to future posts <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

