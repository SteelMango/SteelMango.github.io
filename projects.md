---
layout: page
title: Projects
permalink: /projects/
---

## Cyber Security

{% for post in site.categories.cybersecurity %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %Y" }}
{% endfor %}

## Hardware

{% for post in site.categories.hardware %}
- [{{ post.title }}]({{ post.url }}) — {{ post.date | date: "%b %Y" }}
{% endfor %}