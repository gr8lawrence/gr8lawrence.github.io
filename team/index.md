---
title: Colleagues/Friends
nav:
  order: 3
  tooltip: About my colleagues and close friends and what they are up to
---

# {% include icon.html icon="fa-solid fa-users" %}Colleagues & Friends

Passage 1

{% include section.html %}

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ^(?!pi$)" %}

{% include section.html background="images/background.jpg" dark=true %}

Passage 2
{% include section.html %}

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
