---
layout: page
permalink: /teaching/
title: Teaching
description: 
teachyears: [2021]
tutyears: [2020]
---

<h4>Courses </h4>
{% for y in page.teachyears %}
  <h4 class="year">{{y}}</h4>
  {% bibliography -f teaching -q @*[year={{y}}]* %}
{% endfor %}

<h4>Tutorials </h4>
{% for y in page.tutyears %}
  <h4 class="year">{{y}}</h4>
  {% bibliography -f tutorials -q @*[year={{y}}]* %}
{% endfor %}

