---
layout: page
permalink: /publications/
title: publications
description: Publications by year in reverse chronological order.
years: [2026, 2025, 2024, 2023, 2021, 2019, 2018, 2015]
nav: true
---
<!-- _pages/publications.md -->

<div class="publications">

{%- for y in page.years %}

<h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
