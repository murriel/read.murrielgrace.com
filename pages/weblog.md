---
title: Weblog
layout: collection
menu: true
order: 7
---
<!-- unintended behaviors? --> 
test 0528.04 added site.docs instead

<p>
    {% assign sorted = site.documents | sort: "date" | reverse %}
    {% for item in sorted %}
        <ul>
          <li>
          <a href="{{ item.url | relative_url }}" class="h2 flip-title">  
            <span>{{ item.title }}</a><br /><br /></span>
          <time class="heading faded fine minicap">
          {{ item.date | date_to_string }}</time>  
          <span class="heading faded fine minicap">[{{ item.collection }}]<br /></span>
          <span class="faded fine">{{ item.description }}</span>
          <br /><br />
          </li>
        </ul>
    {% endfor %}

</p>

{% for item in site.collections %}
  <p>
    minitest
    <span>
       <a href="{{ item.url | relative_url }}" class="h2 flip-title">  
           {{ item.title }}</a>
    </span>
  </p>
  
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

