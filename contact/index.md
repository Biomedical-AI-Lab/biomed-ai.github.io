---
title: Contact
nav:
  order: 7
  tooltip: Email, address and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

{% assign brand = site.data.affiliation %}

Email is the best way to reach Prof. Albert.

{%
  include button.html
  type="email"
  text=site.links.email
  link=site.links.email
%}
{%
  include button.html
  type="address"
  text="Directions on Google Maps"
  link=brand.address.map
%}

{% include section.html %}

## Visit

**{{ site.title }}**
{{ brand.address.building }}, {{ brand.address.rooms }}
{{ brand.address.street }}
{{ brand.address.city }}

Prospective students: please come to an [open house]({{ "join" | relative_url }}) rather than visiting unannounced.
