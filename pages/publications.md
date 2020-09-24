---
title: Publications
layout: collection
slug: publications
menu: true
order: 4
description: >
  digital and analog archives from various publications.
---

<p>
  {% for publication in site.publications %}
    <ul>
      <li>
         <a href="{{ publication.url | relative_url }}" class="flip-title">
         <span>{{ publication.title }}</span></a><br/>
         {{ publication.description }}
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>