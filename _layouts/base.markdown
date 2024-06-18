---
title: "Butler's Bank"
meta_description: "Butler's Bank"
activeP: true
---
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>{{ page.title }}</title>
    {% include meta.markdown %}
    <link rel="stylesheet" href="{{ '/assets/css/normalize.css' | relative_url }}">
    <link rel="stylesheet" href="{{ '/assets/css/main.css' | relative_url }}">
    <link rel="stylesheet" href="{{ '/assets/css/responsive.css' | relative_url }}">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  </head>
  <body>
    <header style="background:none;border:none;">
      <a href="{{ '/' | relative_url }}" id="logo_home" style="text-decoration:none;">
        <img src="{{ '/assets/images/butlersbank-logo.png' | relative_url }}" alt="Butler's Bank"/>
        <div id="name_home">
          <div id="logo_top"><h1>BUTLER'S BANK</h1></div>
          <h2>Ne me quitte pas.</h2>
        </div>
      </a>
      <div class="clearfix"></div>
      <nav>
        <ul>
          <li><a href="{{ '/about' | relative_url }}" {% if page.activeA %}class="selected"{% endif %}>ABOUT</a></li>
          <li><a href="{{ '/transportation' | relative_url }}" {% if page.activeP %}class="selected"{% endif %}>TRANSPORTATION</a></li>
          <li><a href="{{ '/cell-phones' | relative_url }}" {% if page.activeR %}class="selected"{% endif %}>CELL PHONES</a></li>
          <li><a href="{{ '/contact' | relative_url }}" {% if page.activeC %}class="selected"{% endif %}>CONTACT</a></li>
        </ul>
      </nav>
    </header>
    <div id="wrapper">
      {{ content }}
      <!-- stick footer-->
      <div class="push"></div>
    </div><!--/.wrapper-->
    <footer>
      <p>&copy; {{ 'now' | date: "%Y" }} Butler's Bank</p>
      <a href="{{ '/contact' | relative_url }}"><img src="{{ '/assets/images/butlersbank-logo.png' | relative_url }}" alt="Butlers Banks Logo" class="social-icon"></a>
    </footer>
    <!-- Google tag (gtag.js) -->
    <!-- End Google tag -->
  </body>
</html>
