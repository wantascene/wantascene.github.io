---
layout: horizontal
title:  "Portrait"
date:   2016-07-10 14:02:15 +0900
categories: gallery
---

{% loop_directory directory:portrait iterator:image filter:*.jpg sort:descending %}
   <li><img src="{{site.url}}/portrait/{{ image }}.jpg" /></li>
{% endloop_directory %}