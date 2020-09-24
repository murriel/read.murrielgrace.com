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
      <!-- do a proper li class later-->
      <li style="margin:0 0 50px 0;">
        <a href="{{ item.url | relative_url }}" class="h2 flip-title">
        <span>{{ item.title }}</a><br /> 
        <time class="heading faded fine">
        {{ item.date | date_to_string }}</time><br />  
        {{ item.description }}</span>
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>