---
layout: page
permalink: /publications/
title: Publications
description:
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

<p>The publications listed on this page represent the full set of my scientific works published to date, including articles from both my current role in industry and my previous research during the PhD at TU Dresden. Together, they reflect the continuity of my research across academia and industry, covering topics in 5G/6G network architecture, IMS, data collection, AI/ML-enabled systems, in-network computing, and next-generation end-to-end user plane design.</p>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>