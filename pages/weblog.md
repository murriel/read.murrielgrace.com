---
title: Weblog
layout: collection
menu: true
order: 7
---
<!-- unintended behaviors? --> 
test 0528.02 change spans etc 

{% for item in site.collections %}
  <ul><li>
         
 <p>minitest<span><a href="{{ item.url | relative_url }}" class="h2 flip-title">  
           {{ item.title }}</a><br /><br /> </span>
  </li></ul>
   {% endfor %}


 {% for item in site.collections %}
  <p><span>
        <ul>
          <!-- do a proper li class later-->
          <li> 
          <span><a href="{{ item.url | relative_url }}" class="h2 flip-title">  
           {{ item.title }}</a><br /><br /> </span>
          <time class="heading faded fine minicap">
          {{ item.date | date_to_string }}</time>  
          <span class="heading faded fine minicap">[{{ item.collection }}]<br /></span>
          <span class="faded fine">{{ item.description }}</span>
          </li> 
        </ul>
 </span></p>
    {% endfor %}

