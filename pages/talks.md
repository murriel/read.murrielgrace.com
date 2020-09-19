---
title: Talks
layout: collection
slug: talks
menu: true
order: 3
description: >
  conference and meetup talks
---

<p>
  {% assign sorted = site.talks | sort: 'date' | reverse %}
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
