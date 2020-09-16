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
  {% assign sorted = (site.posts | sort: 'date') | reverse %}
  {% for item in sorted %}
    <ul>
      <li>
         <span>[{{ item.collection }}]</span><br />
         <a href="{{ item.url | relative_url }}" class="flip-title">
         <span>{{ item.title }}</span></a><br/>
         <span>{{ item.description }}
         {{ item.date }}</span>
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>
