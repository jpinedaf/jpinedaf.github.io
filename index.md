---
layout: default
title: "Home"
permalink: /
wide: true
---

{% assign d = site.data.site %}

<section class="hero">
  <div class="container">
    <h1>{{ site.title }}</h1>
    <p class="tagline">Star formation, gas kinematics and astrochemistry</p>
    <p class="affil">{{ site.position }}, <a href="{{ site.affiliation_link }}" rel="noopener">{{ site.affiliation }}</a></p>
    <p class="intro">I study how stars and planets form, from molecular clouds down to protoplanetary disks, using gas kinematics to understand the physics and astrochemistry to guide and interpret observations.</p>
    <a class="btn" href="{{ '/research/' | relative_url }}">Research</a>
    <a class="btn secondary" href="{{ '/publications/' | relative_url }}">Publications</a>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2>Research themes</h2>
    <div class="cards">
      {% for t in d.themes %}
      <div class="card">
        <img src="{{ t.image | relative_url }}" alt="{{ t.title }}">
        <div class="body"><h3>{{ t.title }}</h3><p>{{ t.text }}</p></div>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<section class="section alt">
  <div class="container">
    <h2>Research programs</h2>
    <div class="cards">
      {% for p in d.programs %}
      <a class="card link-card" href="{{ p.url }}" rel="noopener" style="color: inherit;">
        <div class="body"><h3>{{ p.title }} <i class="fa-solid fa-arrow-up-right-from-square" style="font-size:0.8em"></i></h3><p>{{ p.text }}</p></div>
      </a>
      {% endfor %}
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2>Selected publications</h2>
    <ul class="pub-list">
      {% for p in site.data.publications.main %}{% if p.selected %}
      <li><a href="{{ p.pdf }}" rel="noopener">{{ p.title }}</a><div class="venue">{{ p.venue }}</div></li>
      {% endif %}{% endfor %}
    </ul>
    <p class="more"><a href="{{ '/publications/' | relative_url }}">All publications &rarr;</a> &middot; <a href="{{ site.ads_link }}" rel="noopener">ADS library</a></p>
  </div>
</section>

<section class="section alt">
  <div class="container">
    <h2>Recent highlights</h2>
    <ul class="highlights">
      {% for h in d.highlights %}
      <li><span class="date">{{ h.date }}</span><span><a href="{{ h.url }}" rel="noopener">{{ h.text }}</a></span></li>
      {% endfor %}
    </ul>
  </div>
</section>

<section class="section">
  <div class="container">
    <h2>Software &amp; resources</h2>
    <div class="cards">
      {% for s in d.software %}
      <a class="card link-card" href="{{ s.url }}" rel="noopener" style="color: inherit;">
        <div class="body"><h3><i class="fab fa-github"></i> {{ s.title }}</h3><p>{{ s.text }}</p></div>
      </a>
      {% endfor %}
    </div>
    <p class="more"><a href="{{ '/software/' | relative_url }}">All software &rarr;</a></p>
  </div>
</section>
