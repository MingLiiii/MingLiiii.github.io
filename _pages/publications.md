---
layout: page
permalink: /publications/
title: publications
description: selected publications at top venues, together with a few of my favorite preprints
nav: true
nav_order: 2
---

<div class="publications">
  {% include publication_summary.liquid %}

  <h2>favorite preprints</h2>
  {% bibliography --query @*[favorite=true] --group_by none --sort_by eprint --order descending %}

  <h2>selected publications</h2>
  {% bibliography --query @*[selected=true] --group_by none --sort_by arxiv --order descending %}

</div>
