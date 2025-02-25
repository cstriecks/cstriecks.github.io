---
layout: page
permalink: /talks/
title: talks
description: Given talks in reversed chronological order.
years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2015, 2014, 2013]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f cs-talks -q @*[year={{y}}]* %}
{% endfor %}

</div>