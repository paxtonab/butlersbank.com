---
layout: base
title: "Butler's Bank, GmbH Portfolio"
permalink: /portfolio/
meta_description: "Butler's Bank, GmbH Portfolio"
activeP: true
---

  <section>
    <ul id="gallery">
    {% for item in site.gallery %}
      <li>
        <a href="{{ item.permalink | relative_url }}">
          <img src="{{ item.img_small | relative_url }}" alt="{{ item.title }}">
          <p>{{ item.title }}</p>
        </a>
      </li>
    {% endfor %}
    </ul>
  </section>
