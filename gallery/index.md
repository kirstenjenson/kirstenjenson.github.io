---
layout: default
title: Gallery
images:
    - "000"
    - "001"
    - "002"
    - "003"
    - "004"
    - "005"
    - "006"
    - "007"
    - "008"
    - "009"
    - "010"
    - "011"
    - "012"
    - "013"
    - "014"
    - "015"
    - "016"
    - "017"
    - "018"
    - "019"
    - "020"
    - "021"
    - "022"
    - "023"
    - "024"
    - "025"
---
<ul class="gallery">
{% for image in page.images %}
    {% capture image_url %}{{ site.url }}/img/gallery/{{ image }}{% endcapture %}
    <li><a href="{{ image_url }}.jpg" rel="lightbox[gallery]"><img src="{{ image_url }}_thumb.jpg" alt=""/></a></li>
{% endfor %}
</ul>
