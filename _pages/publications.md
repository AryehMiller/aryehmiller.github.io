---
layout: page
permalink: /publications/
title: publications
description:
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">
  <div class="thumbnail">
    <img src="{{ https://github.com/AryehMiller/aryehmiller.github.io }}/assets/img/TREE_Cover.jpg" alt="Image Description">
    <img src="master/assets/img/CopeiaJPEG.jpg">
    <img src="master/assets/img/PsammodynastescoverJPEG.jpg">
  </div>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
  
</div>
