---
title: Podcast
nav:
  order: 5
  tooltip: Listen to our podcast!
---

# {% include icon.html icon="fa-solid fa-feather-pointed" %}Let's Get Clinical!
<span style="font-size: 20px;">
Currently studying a medical, dental or medical adjacent subject and are wondering what careers are out there for you?
Join us as we welcome a diverse series of special guests to tell you all about the world of clinical academia! We give an honest platform to discuss topics such as inclusivity and diversity in the medical/dental field. 
</span>


<div style="max-width: 100%; display: inline-block;">
  {% include feature.html image="images/LGC_Logo.jpeg" %}
</div>


{% include section.html %}

{% include search-box.html %}

{% include tags.html tags=site.tags %}

{% include search-info.html %}

{%
  include post-excerpt.html
  lookup="Podcast coming soon!"
%}

{% include list.html data="episodes" component="episode-excerpt" %}
