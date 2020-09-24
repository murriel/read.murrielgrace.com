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
      <!-- do a proper li class later-->
      <li style="margin:0 0 50px 0;">
        <span><a href="{{ item.url | relative_url }}" class="h2 flip-title">
        {{ item.title }}</a><br /><br /></span>
        <time class="heading faded fine minicap">
        {{ item.date | date_to_string }}</time><br />  
        <span class="faded fine">{{ item.excerpt }}</span>
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>