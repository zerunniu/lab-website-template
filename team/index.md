---
title: Team
nav:
  order: 3
  tooltip: About our team
---
#  {% include icon.html icon="fa-solid fa-users" %}Team

Here are some descriptions.

{% include section.html %}

## Lab Director

{% include list.html data="members" component="portrait" filter="role == 'professor'" %}

## PhD

{% include list.html data="members" component="portrait" filter="role == 'phd'" %}

## MPhil

{% include list.html data="members" component="portrait" filter="role == 'mphil'" %}

## Research Pathway

{% include list.html data="members" component="portrait" filter="role == 'research-pathway'" %}

## Honours

{% include list.html data="members" component="portrait" filter="role == 'honours'" %}

## Alumni

{% include list.html data="members" component="portrait" filter="role == 'alumni'" %}

{% include section.html background="images/background.jpg" dark=true %}

Here are some descriptions.

{% include section.html %}

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
