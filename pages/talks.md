---
title: Talks
layout: collection
slug: talks
menu: true
order: 3
description: >
  conference and meetup talks
accent_image:
  background: rgba(0,0,0,0.85)
  overlay:    false
---

<p>
  {% for talk in site.talks %}
    <ul>
      <li>
         <a href="{{ talk.url | relative_url }}" class="flip-title">
         <span>{{ talk.title }}</span></a><br/>
         {{ talk.description }}
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>
