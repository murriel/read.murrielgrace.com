---
title: Posts
layout: post
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
         <span><a href="{{ item.url | relative_url }}" class="flip-title">{{ item.title }}</a><br/><br /></span>
         <span class="faded fine">{{ item.excerpt }}</span>
         <span><a href="{{ item.url | relative_url }}" class="faded fine">more >></a></span>
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>

<!-- this is probably gratuitous use of span tags but i'll leave it for now until i figure out a better way (you mean there's a better way??) also the stacked br tags are gross -->