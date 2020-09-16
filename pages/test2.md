---
title: Talky Talk
layout: collection
slug: this is a test
menu: true
order: 3
description: >
  jkjkeyll
---

<p>
  {% assign sorted = (site.pages | sort: 'date') | reverse %}
  {% for item in sorted %}
    <ul>
      <li>
         <a href="{{ item.url | relative_url }}" class="flip-title">
         <span>{{ item.title }}</span></a><br/>
         {{ item.description }}
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>
