---
layout: page
permalink: /publications/
title: publications
description: 
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017]
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->
<div class="publications">

See <a href="https://scholar.google.com/citations?hl=zh-CN&user=qTwd1aEAAAAJ&view_op=list_works&sortby=pubdate" style="color:#b31aaa;">Google Scholar</a> for a full publication list.

<!-- {% bibliography -f {{site.scholar.bibliography}} %} -->

{%- for y in page.years %}
  <h2 class="year" style="color: coral">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
