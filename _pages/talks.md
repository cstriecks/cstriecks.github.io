---
layout: page
permalink: /talks/
title: talks
description: Recent talks (since end of 2018) in reversed chronological order.
years: [2021, 2020, 2019, 2018]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f cs-talks -q @*[year={{y}}]* %}
{% endfor %}

</div>