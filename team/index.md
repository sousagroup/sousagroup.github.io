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

{% assign active_members = members | where: "status", "active" %}

{% assign pi_members = active_members | where: "role", "pi" %}
{% assign sorted_pi_members = pi_members | sort: "name" %}

{% assign phd_students = active_members | where: "role", "phd_student" %}
{% assign sorted_phd_students = phd_students | sort: "name" %}

{% assign mclindent_students = active_members | where: "role", "mclindent" %}
{% assign sorted_mclindent_students = mclindent_students | sort: "name" %}

{% assign undergrad_students = active_members | where: "role", "undergrad" %}
{% assign sorted_undergrad_students = undergrad_students | sort: "name" %}

{% assign sorted_active_members = sorted_pi_members | concat: sorted_phd_students | concat: sorted_mclindent_students | concat: sorted_undergrad_students %}

{% for member in sorted_active_members %}
    {% include list.html data="members" component="portrait" %}
{% endfor %}

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

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
