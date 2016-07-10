---
layout: horizontal
title:  "Portrait"
date:   2016-07-10 14:02:15 +0900
categories: gallery
---

{% for file in site.portrait %}
  {% assign pageurl = page.url | replace: 'index.html', '' %}
  {% if file.path contains pageurl %}
    {% if file.extname == '.jpg' or file.extname == '.jpeg' or file.extname == '.JPG' or file.extname == '.JPEG' %}
    <li><img src="{{ file.path }}" /></li>
    {% endif %}
  {% endif %}
{% endfor %}