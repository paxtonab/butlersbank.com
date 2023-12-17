---
layout: base
title: "Butlers Bank, GmbH"
meta_description: "Butler's Bank, GmBH is a Swiss company focused on supporting the arts through technology."
---

<section id="home-banner">
  <ul id="home-gallery">
    {% for silver in site.silver_gallery %}
      {% if silver.index == 1 or silver.index == 2 or silver.index == 3 %}
      <li>
        <a href="{{ silver.permalink | relative_url }}">
          <img src="{{ silver.img | relative_url }}" alt="{{ silver.title }}">
        </a>
      </li>
      {% endif %}
    {% endfor %}
  </ul>
</section>
