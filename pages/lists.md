---
title: Lists
layout: collection
slug: lists
show_collection: lists
menu: true
order: 5
description: >
  ordered and unordered lists, sometimes arrays, with occasional key value pairs or maps thrown in for fun or profit.
# uncomment to remove accent image
# accent_image:  
#  background: rgba(0,0,0,0.85)
#  overlay:    false
---

<p>
  {% for list in site.lists %}
    <ul>
      <li>
         <span><a href="{{ list.url | relative_url }}" class="h2 flip-title">
         {{ list.title }}</a><br/><br /></span>
         <span class="faded fine">{{ list.description }}</span>
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>
