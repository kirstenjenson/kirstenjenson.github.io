---
layout: default
title: Gallery
images:
    - g000
    - g001
    - g002
    - g003
    - g004
    - g005
    - g006
    - g007
    - g008
    - g009
    - g010
    - g011
    - g012
    - g013
    - g014
    - g015
    - g016
    - g017
    - g018
    - g019
    - g020
    - g021
    - g022
    - g023
    - g024
    - g025
---
<ul class="gallery">
{% for image in page.images %}
    {% capture image_url %}{{ site.url }}/img/gallery/{{ image }}{% endcapture %}
    <li><a href="{{ image_url }}.jpg" rel="lightbox[gallery]"><img src="{{ image_url }}_thumb.jpg" alt=""/></a></li>
{% endfor %}
</ul>
