---
title: Projects
layout: collection
slug: projects
menu: true
order: 2
description: >
  pardon the sawdust, scraps of burnt toast and PLA, dusty typewriter keys, and frayed wires. this is a work in progress.
---

<p>
  {% for project in site.projects %}
    <ul>
      <li>
         <a href="{{ project.url | relative_url }}" class="flip-title">
         <span>{{ project.title }}</span></a><br/>
         {{ project.description }}
      </li>
    </ul>
    <hr>
  {% endfor %}
  </p>


<!-- TEMPORARY  -->
<span class="h2">
  <a href="https://www.murrielgrace.com/m/" target="_blank">Work Projects</a>
  <br /><br />
  <a href="{{ site.url }}/pages/now">Now List</a>
</span>
