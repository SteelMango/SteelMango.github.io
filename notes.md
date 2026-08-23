---
layout: page
title: Notes
permalink: /notes/
---

{% for post in site.categories.notes %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %Y" }}
{% endfor %}
