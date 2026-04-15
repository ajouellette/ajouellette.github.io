---
layout: page
permalink: /publications/
title: Publications
description:
years: [2025, 2024, 2023]
nav: true
nav_order: 1
---

Check out [NASA ADS](https://ui.adsabs.harvard.edu/public-libraries/8HO4FBxpSfaSnWv-88mkyA)
or [Google Scholar](https://scholar.google.com/citations?user=hLz6cJQAAAAJ&hl=en)
for the full list of publications that I contributed to.

## First-author publications:
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
