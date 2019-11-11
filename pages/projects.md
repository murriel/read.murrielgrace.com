---
title: Projects
layout: collection
slug: projects
menu: true
order: 2
description: >
  pardon the sawdust, scraps of burnt toast and PLA, dusty typewriter keys, and frayed wires. this is a work in progress.
accent_color: rgb(38,139,210)
accent_image:
  background: rgb(32,32,32)
  overlay:    false
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
