---
title: Talks
layout: collection
slug: talks
menu: true
order: 3
description: >
  conference and meetup talks
accent_color: rgb(38,139,210)
accent_image:
  background: rgb(32,32,32)
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
