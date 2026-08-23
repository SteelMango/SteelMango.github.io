---
layout: page
title: Projects
permalink: /projects/
---

## Cyber Security

<ul class="post-list">
{%- for post in site.categories.cybersecurity -%}
  <li class="post-list-item">
    <a class="post-thumbnail-link" href="{{ post.url | relative_url }}">
      {%- if post.image -%}
      <img class="post-thumbnail" src="{{ post.image | relative_url }}" alt="{{ post.title | escape }}">
      {%- else -%}
      <div class="post-thumbnail post-thumbnail--placeholder"></div>
      {%- endif -%}
    </a>
    <div class="post-list-text">
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
      <span class="post-meta">{{ post.date | date: "%b %Y" }}</span>
    </div>
  </li>
{%- endfor -%}
</ul>

## Hardware

<ul class="post-list">
{%- for post in site.categories.hardware -%}
  <li class="post-list-item">
    <a class="post-thumbnail-link" href="{{ post.url | relative_url }}">
      {%- if post.image -%}
      <img class="post-thumbnail" src="{{ post.image | relative_url }}" alt="{{ post.title | escape }}">
      {%- else -%}
      <div class="post-thumbnail post-thumbnail--placeholder"></div>
      {%- endif -%}
    </a>
    <div class="post-list-text">
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3>
      <span class="post-meta">{{ post.date | date: "%b %Y" }}</span>
    </div>
  </li>
{%- endfor -%}
</ul>
