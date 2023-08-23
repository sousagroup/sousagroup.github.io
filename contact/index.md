---
title: Contact
nav:
  order: 5
  tooltip: Reach out to our team
---

# {% include icon.html icon="fa-regular fa-envelope" %}Get In Touch

Dive deep into the crossroads of oral health and systemic diseases. Let's explore together.

{%
  include button.html
  type="email"
  text="vanessa.sousa@kcl.ac.uk"
  link="vanessa.sousa@kcl.ac.uk"
%}
{%
  include button.html
  type="phone"
  text="07788201109"
  link="+447788201109"
%}
{%
  include button.html
  type="address"
  tooltip="Navigate to our research hub"
  link="https://www.google.com/maps/place/Guy's+Hospital/@51.5031934,-0.0893986,17z/data=!3m1!4b1!4m6!3m5!1s0x48760357591cb78b:0x20bad9c140ba3c61!8m2!3d51.5031901!4d-0.0868237!16zL20vMDJjM3Jq?entry=ttu"
%}

{% include section.html %}

{% capture col1 %}
{%
  include figure.html
  image="images/team_photo.jpg"
  caption="Passionate minds at KCL Lab."
%}
{% endcapture %}

{% capture col2 %}
{%
  include figure.html
  image="images/equipment_photo.jpg"
  caption="Innovation in every detail."
%}
{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

{% capture col1 %}
Deep in the heart of London, at KCL, we embark on a journey to decode the mysteries linking oral health with systemic diseases. Every study, every test, every discovery takes us a step closer to redefining healthcare for all.
{% endcapture %}

{% capture col2 %}
Your curiosity, expertise, and passion can fuel our mission. Join us on this enlightening journey, and together, let's illuminate the unknown. The future of holistic health research awaits.
{% endcapture %}

{% capture col3 %}
Keep your pulse on the latest from our lab. Subscribe to updates, share in our discoveries, and be a part of the conversation. A world of groundbreaking insights awaits.
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
