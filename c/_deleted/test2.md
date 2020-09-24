---
title: Talky Talk
layout: collection
slug: this is a test
menu: true
order: 3
description: >
  jkjkeyll
---
<h1>zoro zero</h1>

<p>
{% assign sortedcol = site.documents | sort: 'date' | reverse %}
{% for item in sortedcol limit:20 %}
    <ul>
      <li>
      <span><b>[{{ item.collection }}]</b></span>
      <a href="{{ item.url | relative_url }}" class="h4 flip-title">
        <span>{{ item.title }}</span></a>
      <time class="heading faded fine">
      {{ item.date | date_to_string }}</time>
      </li>
    </ul>
{% endfor %}
</p>


<hr>
<hr>

<h1>un</h1>
{% for collection in site.collections %}
  <h2>Items from {{ collection.label }}</h2>
  <ul>
    {% for item in site[collection.label] %}
      <li><a href="{{ item.url }}">{{ item.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
<hr>

<h2>deux</h2>
<p>
  {% assign sorted = site.posts | sort: 'date' | reverse %}
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
