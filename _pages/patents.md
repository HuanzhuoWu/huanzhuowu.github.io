---
layout: page
permalink: /patents/
title: Patents
description:
years: [2025, 2024]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

<p>This page includes only my publicly disclosed patents, as published through international or national patent offices. Many of my patent applications are still under review and therefore remain confidential until their respective publication dates. As a result, the list below does not represent the full scope of my patent portfolio, but only the subset that is currently accessible in the public domain. This page will be updated continuously as additional applications become publicly available.</p>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f patents -q @*[year={{y}}]* %}
{% endfor %}

</div>