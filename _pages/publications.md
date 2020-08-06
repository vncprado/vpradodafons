---
layout: page
permalink: /publications/
title: publications
description: Recent publications.
years: [2019, 2018, 2017, 2015, 2014]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
