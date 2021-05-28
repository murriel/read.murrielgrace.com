---
title: Weblog
layout: weblog
menu: true
order: 1
---
<!-- unintended behaviors ? --> 
<p>
 {% for item in site.documents %}
        <ul>
          <!-- do a proper li class later-->
          <li> 
          <span><a href="{{ item.url | relative_url }}" class="h2 flip-title">  
           {{ item.title }}</span></a><br /><br /> 
          <time class="heading faded fine minicap">
          {{ item.date | date_to_string }}</time>  
          <span class="heading faded fine minicap">[{{ item.collection }}]<br /></span>
          <span class="faded fine">{{ item.description }}</span>
          </li>
        </ul>
    {% endfor %}
</p>
