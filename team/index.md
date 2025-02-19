---
title: Creators
nav:
  order: 3
  tooltip: The people who made this site!
---

# {% include icon.html icon="fa-solid fa-users" %} Current and past contributors

<span style="font-size: 20px;">
Our lab is a lively and diverse collective, with members from various corners of the globe. Including people from all over the world we hope to be as inclusive as possible as we continue our research journey. The team is made up of specialised dentists and students of all levels!
</span>

{% include section.html %}

# Creators 

{% include list.html data="members" component="portrait" filters="status: active, role: pi" %}
{% include list.html data="members" component="portrait" filters="status: active, role: phd" %}
{% include list.html data="members" component="portrait" filters="status: active, role: mclindent" %}
{% include list.html data="members" component="portrait" filters="status: active, role: undergrad" %}
{% include list.html data="members" component="portrait" filters="status: active, role: mascot" %}

{% include section.html %}

# Past Contributors

<span style="font-size: 20px;">
Have a look at some of the wonderful people who have worked on this project in the past. We keep in touch with alumni and keep them in the loop of our current progress!
</span>

{% include list.html data="members" component="portrait" filters="status: alumni" %}

{% include section.html %}

# Project Mascot

<span style="font-size: 20px;">
Our project mascot Rosita always brings great energy!
</span>

{% include list.html data="members" component="portrait" filters="status: mascot" %}

{% include section.html background="images/background.jpg" %}

We are always looking for new members! Please look on findaphd.com to see if we are advertising or email us directly!

{% include section.html %}

{% capture content %}

{% include figure.html image="images/clinic.jpeg" caption="On the clinic with the peri-implantitis team!" %}
{% include figure.html image="images/joe_presenting.jpeg" caption="Joe presenting in Chile to our collaborators" %}
{% include figure.html image="images/rosita.jpeg" caption="Rosita!! Our lab mascot!" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
