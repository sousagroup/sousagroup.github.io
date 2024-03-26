---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %} Team

<span style="font-size: 20px;">
Our lab is a lively and diverse collective, with members from various corners of the globe. Including people from all over the world we hope to be as inclusive as possible as we continue our research journey. The team is made up of specialised dentists and students of all levels!
</span>

{% include section.html %}

# Current Team 

{% include list.html data="members" component="portrait" filters="status: active, role: pi" %}
{% include list.html data="members" component="portrait" filters="status: active, role: phd" %}
{% include list.html data="members" component="portrait" filters="status: active, role: mclindent" %}
{% include list.html data="members" component="portrait" filters="status: active, role: undergrad" %}

{% include section.html %}

# Past Members

<span style="font-size: 20px;">
Have a look at some of the wonderful people who have worked in the lab in the past. We keep in touch with alumni and keep them in the loop of our current research!
</span>

{% include list.html data="members" component="portrait" filters="status: alumni" %}

{% include section.html background="images/background.jpg" %}

We are always looking for new members! Please look on findaphd.com to see if we are advertising or email us directly!

{% include section.html %}

{% capture content %}

{% include figure.html image="images/clinic.jpeg" %}
{% include figure.html image="images/joe_presenting.jpeg" %}
{% include figure.html image="images/rosita.jpeg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
