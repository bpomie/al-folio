---
layout: page
permalink: /publications/
title: publications
description: #The articles are posted for non-commercial use only.
years: [preprints, 2022, 2021, 2020, 2019, 2017, 2016, 2015]
nav: true
---

Check also my <a href = "https://scholar.google.com/citations?user=EaZd_hkAAAAJ&hl=pl&oi=ao"> Google Scholar profile</a>.

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
