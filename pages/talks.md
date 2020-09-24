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
  {% for talk in site.talks %}
    <ul>
      <li style="margin:0 0 50px 0;">
        <span><a href="{{ talk.url | relative_url }}" class="h2 flip-title">
        {{ talk.title }}</a><br /><br /></span>
        <time class="heading faded fine minicap">
        {{ talk.date | date_to_string }}</time><br />  
        <span class="faded fine">{{ talk.excerpt }}</span>
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>