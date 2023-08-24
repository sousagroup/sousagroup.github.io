---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

<span style="font-size: 20px;">
Our lab is a lively and diverse collective, with members from various corners of the globe. Including people from all over the world we hope to be as inclusive as possible as we continue our research journey. The team is made up of specialised dentists and students of all levels!
</span>

{% include section.html %}

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ^(?!pi$)" %}

{% include section.html background="images/background.jpg" dark=true %}

We are always looking for new members! Please see below the current PhD/post-doctoral projects advertised by us!

{% include section.html %}

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
