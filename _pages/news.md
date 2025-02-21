---
layout: page
permalink: /news/
title: news
# years: [2023, 2022, 2021, 2020]
nav: true
nav_order: 1
---

<div class="publications">

{%- for y in site.data.news %}
  <h2 class="year">{{y[0]}}</h2>
  <ul>
  {%- for m in y[1] %}
    <li>
      <a href="{{m.url}}">{{m.title}}</a> 
      <i>({{m.organization}})</i>
    </li>
  {% endfor %}
  </ul>
{% endfor %}

</div>


<!-- <div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f news -q @*[year={{y}}]* %}
{% endfor %}

</div> -->