---
layout: page
permalink: /publications-legacy/
title: publications legacy
description: legacy BibTeX-rendered publications page
nav: false
---

<div class="publications">
  {% include publication_summary.liquid %}

  <h2>favorite preprints</h2>
  {% bibliography --query @*[favorite=true] --group_by none --sort_by eprint --order descending %}

  <h2>selected publications</h2>
  {% bibliography --query @*[selected=true] --group_by none --sort_by arxiv --order descending %}

</div>
