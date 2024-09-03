---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Blog
permalink: /blog/
---


<div>
  {% for post in site.posts %}
      <small>{{ post.date | date: "%-d %B %Y" }}</small>
      <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
      {{ post.excerpt }}
     <hr/> 
  {% endfor %}
</div>


<p class="rss-subscribe">subscribete <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>
