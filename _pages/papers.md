---
layout: page
title: papers
permalink: /papers/
nav: true
nav_order: 2
---

<h2>Publications </h2>

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

