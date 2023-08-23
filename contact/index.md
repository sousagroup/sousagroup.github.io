---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

If you find our research interesting and want to get involved or simply just want to learn more then please contact us using the details below!

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
  link="(www.google.com/maps/place/Guy's+Hospital/@51.5031934,-0.0893986,17z/data=!3m1!4b1!4m6!3m5!1s0x48760357591cb78b:0x20bad9c140ba3c61!8m2!3d51.5031901!4d-0.0868237!16zL20vMDJjM3Jq?entry=ttu)"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

{% capture col1 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col2 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col3 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
