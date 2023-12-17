---
layout: base
title: "Butler's Bank, GmbH Portfolio"
permalink: /portfolio/
meta_description: "Butler's Bank, GmbH Portfolio"
activeP: true
---

  <section>
    <ul id="gallery">
    {% for silver in site.silver_gallery %}
      <li>
        <a href="{{ silver.permalink | relative_url }}">
          <img src="{{ silver.img_small | relative_url }}" alt="{{ silver.title }}">
          <p>{{ silver.title }}</p>
        </a>
      </li>
    {% endfor %}
    </ul>
  </section>
