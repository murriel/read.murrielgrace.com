---
title: Weblog
layout: collection
menu: true
order: 7
---
<!-- unintended behaviors? --> 
test 0528.05 working with site.docs

<p>
    {% assign sorted = site.documents | sort: "date" | reverse %}
    {% for item in sorted %}
        <ul>
          <li>
          <span><a href="{{ item.url | relative_url }}" class="h2 flip-title">{{ item.title }}</a></span>
              <span><time class="heading faded fine minicap">
              {{ item.date | date_to_string }}</time></span>
          <span class="heading faded fine minicap">[{{ item.collection }}]<br /></span>
          <span class="faded fine">{{ item.description }}</span>
          <br /><br />
          </li>
        </ul>
    {% endfor %}

</p>
