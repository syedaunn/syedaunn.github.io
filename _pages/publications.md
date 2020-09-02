---
layout: page
permalink: /publications/
title: publications
description: More frequently updated publications can be found at <a href="https://scholar.google.ch/citations?user=iSm-PtcAAAAJ" target="_blank">Google Scholar</a>.<br/><br/>Following publications by categories in reversed chronological order. 
years: [2020, 2019, 2017]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
