---
layout: custom_page
title: Blog
image: 
pagination: 
  enabled: true
---

<h3 class="notes-list-header">All posts</h3>

<ul class="notes-list highlight">
{% assign sorted_notes = site.notes | reverse %}
{% for post in sorted_notes %}
  <li>
    <a class="notes-title" href="{{ post.url }}">{{ post.title }}</a>
    <span class="notes-date">{{ post.date | date: "%b %d, %Y" }}</span>
  </li>
{% endfor %}
</ul>
