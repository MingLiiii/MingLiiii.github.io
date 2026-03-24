---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
nav: true
nav_order: 2
---

<div class="publications">
  {% include publication_summary.liquid %}

  <h2>selected publications</h2>
  {% bibliography --query @*[selected=true] --group_by none %}

  <h2>favorite preprints</h2>
  {% bibliography --query @*[favorite=true] --group_by none %}

</div>
