---
layout: page
title: "Work"
permalink: /work/
---

Professional projects.

<ul class="post-list">
  {%- for work in site.work -%}
  <li>
    <h3>
      <a class="post-link" href="{{ work.url | remove: '.html' | relative_url }}">
        {{ work.title | escape }}
      </a>
    </h3>
    <span class="post-meta">{{ work.short_description | markdownify }}</span>
  </li>
  {%- endfor -%}
</ul>

Check [my CV]({% link cv.md %}) for a list of other projects and get in touch with me on [LinkedIn](http://www.linkedin.com/in/neildawson) if you'd like to know more.