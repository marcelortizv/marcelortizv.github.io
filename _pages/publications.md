---
layout: page
permalink: /publications/
title: Research
description: Publications & Working Papers
years: [2024]
nav: true
nav_order: 2
---

<div class="publications">

<h3>Working papers</h3>
{% bibliography -f preprints %}


<h3>Publications</h3>

{%- for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}


</div>
