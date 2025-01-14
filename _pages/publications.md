---
layout: page
permalink: /publications/
title: Publications
description:
gyears: [2025, 2024] 
ugyears: [2022, 2021, 2020, 2018]
hsyears: [2013]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<h4>Graduate</h4>
{%- for y in page.gyears %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f gpapers -q @*[year={{y}}]* %}
{% endfor %}

<br>

<h4>Undergraduate</h4>
{%- for y in page.ugyears %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f ugpapers -q @*[year={{y}}]* %}
{% endfor %}

<br>

<h4>High School</h4>
{%- for y in page.hsyears %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f hspapers -q @*[year={{y}}]* %}
{% endfor %}

</div>
