---
layout: page
title: "Play"
permalink: /play/
---

Personal projects.

<ul class="post-list">
  {%- for play in site.play -%}
  <li>
    <h3>
      <a class="post-link" href="{{ play.url | relative_url }}">
        {{ play.title | escape }}
      </a>
    </h3>
    <span class="post-meta">{{ play.short_description | markdownify }}</span>
  </li>
  {%- endfor -%}
</ul>