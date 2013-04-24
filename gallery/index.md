---
layout: default
title: Gallery
images:
    - !str 000
    - !str 001
    - !str 002
    - !str 003
    - !str 004
    - !str 005
    - !str 006
    - !str 007
    - !str 008
    - !str 009
    - !str 010
    - !str 011
    - !str 012
    - !str 013
    - !str 014
    - !str 015
    - !str 016
    - !str 017
    - !str 018
    - !str 019
    - !str 020
    - !str 021
    - !str 022
    - !str 023
    - !str 024
    - !str 025
---
<ul class="gallery">
{% for image in page.images %}
    {% capture image_url %}{{ site.url }}/img/gallery/{{ image }}{% endcapture %}
    <li><a href="{{ image_url }}.jpg" rel="lightbox[gallery]"><img src="{{ image_url }}_thumb.jpg" alt=""/></a></li>
{% endfor %}
</ul>
