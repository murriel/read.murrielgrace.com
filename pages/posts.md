---
title: Posts
layout: collection
menu: true
order: 1
description: >
  projects, thoughts, errata, and addendums.
---

<p>
  {% assign sorted = site.posts | sort: 'date' | reverse %}
  {% for item in sorted %}
    <ul>
      <li>
         <a href="{{ item.url | relative_url }}" class="flip-title">
         <span>{{ item.title }}</span></a><br/>
         <i>{{ item.description }}</i>
         {{ item.excerpt }}
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>