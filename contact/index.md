---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

If you find our research intriguing or wish to delve deeper into the connections between oral health and systemic diseases, please reach out to us.

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
  tooltip="Our location on Google Maps for easy navigation"
  link="https://www.google.com/maps/place/Guy's+Hospital/@51.5031934,-0.0893986,17z/data=!3m1!4b1!4m6!3m5!1s0x48760357591cb78b:0x20bad9c140ba3c61!8m2!3d51.5031901!4d-0.0868237!16zL20vMDJjM3Jq?entry=ttu"
%}

{% include section.html %}

{% capture col1 %}
{%
  include figure.html
  image="images/team_photo.jpg"
  caption="Members of our team at work in the KCL lab."
%}
{% endcapture %}

{% capture col2 %}
{%
  include figure.html
  image="images/equipment_photo.jpg"
  caption="Advanced equipment used for our oral health research."
%}
{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

{% capture col1 %}
Our lab at KCL is committed to unravelling the intricate ties between oral health and systemic diseases. Through rigorous research, we aim to advance medical understanding and offer holistic approaches to health.
{% endcapture %}

{% capture col2 %}
If you're a student, researcher, or healthcare professional interested in contributing to our mission, we always welcome new perspectives. Your expertise can help shape a healthier future.
{% endcapture %}

{% capture col3 %}
Subscribe to our newsletter or follow our social media channels to stay updated with our latest findings, publications, and events. Knowledge shared is a step towards a healthier world.
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
