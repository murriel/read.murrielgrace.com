---
title: Weblog
layout: collection
menu: true
order: 7
---
<!-- unintended behaviors ? --> 
<p>test
 {% for item in site.collections %}
        <ul>
          <!-- do a proper li class later-->
          <li> 
          <span><a href="{{ item.url | relative_url }}" class="h2 flip-title">  
           {{ item.title }}</span></a><br /><br /> 
          <time class="heading faded fine minicap">
          {{ item.date | date_to_string }}</time>  
          <span class="heading faded fine minicap">[{{ item.collection }}]<br /></span>
          <span class="faded fine">{{ item.description }}</span>
          </li>git 
        </ul>
    {% endfor %}
</p>
