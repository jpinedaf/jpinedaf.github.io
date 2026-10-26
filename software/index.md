---
layout: default
title: "Software"
permalink: /software/
---

Research tools developed for the analysis of spectral-line and interferometric data.

<div class="cards">
  {% for s in site.data.site.software %}
  <a class="card link-card" href="{{ s.url }}" rel="noopener" style="color: inherit;">
    <div class="body"><h3><i class="fab fa-github"></i> {{ s.title }}</h3><p>{{ s.text }}</p></div>
  </a>
  {% endfor %}
</div>

Other repositories: [GBT Ammonia Survey](https://github.com/GBTAmmoniaSurvey) &middot; [GitHub profile]({{ site.github_link }})
