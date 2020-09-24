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
         <span><a href="{{ publication.url | relative_url }}" class="h2 flip-title">
         {{ publication.title }}</a><br/><br /></span>
         <span class="faded fine">{{ publication.description }}</span>
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>
