---
title: Colleagues/Friends
nav:
  order: 3
  tooltip: About my colleagues and close friends and what they are up to
---

# {% include icon.html icon="fa-solid fa-users" %}Colleagues & Friends

Glad you made it here - not only can you find my full bio but also read about the life and works of my (human and feline) friends. Enjoy exploring!

{% include section.html %}

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ^(?!pi$)" %}
