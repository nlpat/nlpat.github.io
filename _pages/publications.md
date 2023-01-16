---
layout: page
permalink: /publications/
title: Publications
years: [2022, 2021, 2020, 2019, 2018, 2017]
---

{% for y in page.years %}
  <h5 style='font-family: "Spartan";font-weight:100; text-align: left'>{{y}}</h5>
  <hr style='width: 100%; opacity: 0.45; '>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
