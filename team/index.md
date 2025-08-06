---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Here are some descriptions.

{% include section.html %}

## Professor
{% include list.html data="members" component="portrait" filter="role == 'professor'" %}

## PhD Students
{% include list.html data="members" component="portrait" filter="role == 'phd'" %}

## MPhil Students
{% include list.html data="members" component="portrait" filter="role == 'mphil'" %}

## Research Pathway Students
{% include list.html data="members" component="portrait" filter="role == 'research-pathway'" %}

## Other Students
{% include list.html data="members" component="portrait" filter="role == 'other' or role == 'master' or role == 'research-pathway' or role == 'undergrad'" %}

{% include section.html background="images/background.jpg" dark=true %}

Here are some descriptions.

{% include section.html %}

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
