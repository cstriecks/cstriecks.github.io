---
layout: page
permalink: /publications/
title: publications
description: Author names are listed in alphabetical order depending on their last name (if not indicated otherwise).
years: [2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f cs -q @*[year={{y}}]* %}
{% endfor %}

</div>