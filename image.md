---
layout: page
title: image
permalink: /image
---

四格缩进在markdown会被视为代码块
{% assign image_files = site.static_files | where: "image", true %}
{% for myImage in image_files %}
<img src="{{ myImage.path }}">
{% endfor  %}
