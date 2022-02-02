---
layout: page
permalink: /publications/
title: Publications
img: publications.jpg
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2009, 2008, 2007, 2006, 2005]
---

{% for y in page.years %}
  <h5 style='font-family: "Spartan";font-weight:100; text-align: left'>{{y}}</h5>
  <hr style='width: 100%; opacity: 0.45; '>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
