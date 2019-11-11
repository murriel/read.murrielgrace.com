---
title: Publications
layout: collection
slug: publications
menu: true
order: 4
description: >
  electronic and analog archives
---

<p>
  {% for publication in site.publications %}
    <ul>
      <li>
         <a href="{{ publication.url | relative_url }}" class="flip-title">
         <span>{{ publication.title }}</span></a><br/>
         {{ publication.description }}
      </li>
      <li>
      {{ publication.path }}<br/>
      {{ publication.url }}<br/>
      {{ publication.collection }}
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>
