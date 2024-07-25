---
title: Contact
nav:
  order: 6
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact Us
<span style="font-size: 20px;">
If you find our research intriguing and wish to learn more about the connections between oral health and systemic diseases, please reach out to us!
</span>
<div class="button-group">
  {%
    include button.html
    type="email"
    text="vanessa.sousa@kcl.ac.uk"
    link="vanessa.sousa@kcl.ac.uk"
    class="contact-button"
  %}
  {%
    include button.html
    type="phone"
    text="07788201109"
    link="+447788201109"
    class="contact-button"
  %}
  {%
    include button.html
    type="address"
    tooltip="Our location on Google Maps for easy navigation"
    link="https://www.google.com/maps/place/Guy's+Hospital/@51.5031934,-0.0893986,17z/data=!3m1!4b1!4m6!3m5!1s0x48760357591cb78b:0x20bad9c140ba3c61!8m2!3d51.5031901!4d-0.0868237!16zL20vMDJjM3Jq?entry=ttu"
    class="contact-button"
  %}
</div>

{% include section.html %}

<div class="image-section">
  {% capture col1 %}
  {%
    include figure.html
    image="images/guys2.png"
    caption="We are based in Guy's hospital! (image credit: GSTT photos)"
  %}
  {% endcapture %}
  
  {% capture col2 %}
  {%
    include figure.html
    image="images/rosita2.jpeg"
    caption="Rosita again!!"
  %}
  {% endcapture %}
  
  {% include cols.html col1=col1 col2=col2 %}
</div>

{% include section.html %}

<div class="info-section">
  {% capture col1 %}
  Our lab at KCL is deeply invested in understanding the complex interplay between oral health and systemic diseases. We believe that by investigating this relationship, we can pave the way for groundbreaking medical discoveries and contribute to holistic health approaches.
  {% endcapture %}
  
  {% capture col2 %}
  Join our cause! Whether you are a student, a seasoned researcher, or a curious mind, your perspective is valuable. Dive into this research journey with us and let's work together towards a brighter, healthier future.
  {% endcapture %}
  
  {% capture col3 %}
  Stay in the loop with our latest research, findings, and publications. Consider following us on our youtube channels for conference presentations. Together, we can spread knowledge and make strides in the world of health research.
  {% endcapture %}
  
  {% include cols.html col1=col1 col2=col2 col3=col3 %}
</div>
