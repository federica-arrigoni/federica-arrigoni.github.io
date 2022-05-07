---
layout: page
permalink: /publications/
title: Publications
description: 
procyears: [2021, 2020, 2019, 2017, 2016, 2015, 2014]
jouryears: [2022, 2020, 2019, 2018, 2016]
---

<h4>Journals</h4>
{% for y in page.jouryears %}
  <h4 class="year">{{y}}</h4>
  {% bibliography -f journals -q @*[year={{y}}]* %}
{% endfor %}

<h4>Proceedings</h4>
{% for y in page.procyears %}
  <h4 class="year">{{y}}</h4>
  {% bibliography -f proceedings -q @*[year={{y}}]* %}
{% endfor %}

